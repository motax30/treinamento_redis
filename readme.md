# Redis - Um banco de dados em memória para diversos propósitos

## Instalação

Para iniciarmos a utilização do banco de dados em memória Redis precisaremos seguir os seguintes passos

1. Primeiramente precisaremos rodar uma imagem do servidor do banco de dados Redis Alpine executando o comando à seguir:

   ```
   docker run --rm --name test-redis redis:6.2-alpine redis-server --loglevel warning
   ```

   Este comando iniciará um container chamado "test-redis" que terá a instância do servidor de nosso banco de dados para podermos fazer uso do mesmo.
2. Para acessarmos o banco de redis e comecarmos a executar os primeiros comandos podemos rodar o seguinte comando:

   ```
   docker exec -it test-redis redis-cli
   ```
3. Executaremos agora 3 comandos para fazermos um teste

   **KEYS (Verifica as chaves exixtentes); MSET(Persiste um novo valor) e MGET(Recupera um valor do banco de dados)**

   ```
   KEYS *
   ```


   ```
   MSET test "primeiro valor"
   ```


   ```
   MGET test
   ```
4. Para rodar o Redis com mais opções de configuração a sua instanciação via linha de comando ficará inviável, para isso podemos utilizar um arquivo docker-compose chamado "docker-compose-redis.yml" no qual podemos definir algumas configurações adicionais tais como inclusão de persistência e autenticação:

   ```
   version: '3.8'
   services:
     cache:
       image: redis:6.2-alpine
       restart: always
       ports:
         - '6379:6379'
       command: redis-server --save 20 1 --loglevel warning --requirepass eYVX7EwVmmxKPCDmwMtyKVge8oLd2t81
       volumes: 
         - cache:/data
   volumes:
     cache:
       driver: local
   ```

   Aqui nós estamos definindo um serviço chamado cache utilizando um imagem do redis na versão 6.2-alphine que será reestartada sempre, terá um mapeamento para ser acessado pela porta 6379.

   Consequentemente será executado um comando customizado do redis para salvar 1 ou mais linhas a cada 20 segundos no disco no caso do servidor ser reeniciado

   Nós estamos usando o parâmetro `--requirepass` para adicionar autenticação com uma senha para leitur/escrita dos dados no servidor Redis.

   Estamos também utilizando um volume para persistirmos em disco os dados do banco em uma pasta chamada "cache" no caso em que ocorra alguma falha em nosso container.

   Dito isto podemos rodar o arquivo docker-compose acima usando

   ```
   docker-compose -f docker-compose-redis.yml up
   ```

    O container instanciado após a execução do arquivo docker-compose é similar ao container instanciado anteriormente pela linha de comando. As duas maiores diferenças aqui são o volume montado para a persistência dos dados em disco e a senha definida para autenticação dentro do container.

    A frente faremos utilizaremos o banco redis em conjunto a uma aplicação flask utilizando o banco de dados postgres.

# Client para acesso ao Redis

Podemos nos conectar ao Redis das seguintes formas:

* Com a ferramenta de linha de comando nativa "redis-cli"
* Usando o "Redis Insight" uma interface de usuário gráfica
* Via uma biblioteca client para uma linguagem de programação

### Redis Insight

Combina uma API gráfica com a CLI do Redis para que você trabalhe com qualquer implantação de Redis. De forma visual poderemos interagir com o banco de dados fazendo operações nele com a vantagem de possuir como vantagem um conjunto de ferramentas de diagnóstico. E o melhor de tudo, é free.

### Client Libraries

Atualmente temos client para acesso facilitado ao banco de dados em várias linguagens de programação, conforme abaixo:

* [C#/.NET](https://redis.io/docs/latest/develop/connect/clients/dotnet/)
* [Go](https://redis.io/docs/latest/develop/connect/)
* [Java](https://redis.io/docs/latest/develop/connect/clients/java/)
* [Node.js](https://redis.io/docs/latest/develop/connect/clients/nodejs/)
* [Python](https://redis.io/docs/latest/develop/connect/clients/python/)

No nosso caso aqui no treinamento focaremos na utilização do client para python o qual abordaremos com mais detalhes abaixo.

### Python Client for Redis

O client python requer que o servidor do Redis esteja em execução. Vamos iniciar fazendo a instalação do client python seguindo os seguintes passos:

1. Instalando o redis.py fazendo uso do gerenciador de pacotes "pip" do python:

   ```
   pip install redis
   ```
2. Agora precisamos realizar a conexão ao banco Redis com as seguintes configurações:

   ```
   r= redis.Redis(host='localhost', port=6379, decode_response=True)
   ```
3. Agora faremos algumas operações de escrita e leitura de dados:

   ```
   r.set('usuario','Marcos')
   # True
   r.get('usuario')
   # Marcos
   ```
4. Para persistirmos e recuperarmos dicionários:

   ```
   r.hset('dados_usuario1', mapping={
   	'nome': 'Jpão',
   	'Sobrenome':'Fernandes',
   	'empresa':'Google'
   	'idade':'32'
   })
   #True

   r.hgetall('dados_usuario')
   # {'nome': 'Jpão', 'Sobrenome':'Fernandes', 'empresa':'Google' 'idade':'32'}
   ```
5. Vamos agora criar alguns dados de teste para adicionarmos ao nosso banco de dados:

   ```
   user1 = {
       "name": "Paul John",
       "email": "paul.john@example.com",
       "age": 42,
       "city": "London"
   }
   user2 = {
       "name": "Eden Zamir",
       "email": "eden.zamir@example.com",
       "age": 29,
       "city": "Tel Aviv"
   }
   user3 = {
       "name": "Paul Zamir",
       "email": "paul.zamir@example.com",
       "age": 35,
       "city": "Tel Aviv"
   }
   ```
6. Para a definição de indices para os campos e seus tipos de dados podemos utilizar schemas. Utilizamos uma estrutura do tipo JSON para mapear os campos para o schema:

   ```
   schema = (
       TextField("$.name", as_name="name"), 
       TagField("$.city", as_name="city"), 
       NumericField("$.age", as_name="age")
   )
   ```
7. Criado o index, no exemplo abaixo todos os documentos JSON com o prefixo chave "user" serão indexados:

   ```
   rs = r.ft("idx:users")
   rs.create_index(
       schema,
       definition=IndexDefinition(
           prefix=["user:"], index_type=IndexType.JSON
       )
   )
   # b'OK'
   ```
8.
