# Redis - Um banco de dados em memória para diversos propósitos

## O que é o Redis

* O Redis é um **[banco de dados](https://rockcontent.com/br/blog/banco-de-dados/) relacional** de código aberto, que tem como uma de suas principais características o fato de estruturar informações em sua memória.
* Altamente versátil, **o Redis pode ser usado em projetos complexos de TI** que contemplem aplicações web, softwares internos de uma empresa, além de uma série de outras possibilidades.
* Seu funcionamneto extremamente simples utiliza o conceito de “chave/valor” para definição de suas estruturas.
* Um dos fatores mais importantes quanto ao Redis é o fato de ele ser um sistema voltado para o **armazenamento e o processamento mais dinâmico e ágil.**
* Consegue processar dados em uma velocidade muito mais alta do que outras aplicações.
* É um banco de dados capaz de performar bem, mesmo com alto volume de informações.

Em sua utilidade, o Redis pode suportar diferentes estruturas de dados, entre eles:

* strings;
* hashes;
* listas;
* conjuntos;
* conjuntos ordenados com consultas de alcance;
* bitmaps;
* hiperlogs;
* índices geoespaciais;
* streams.

Um dos fatores mais importantes quanto ao Redis é o fato de ele ser um sistema voltado para o **armazenamento e o processamento mais dinâmico e ágil**. Isso significa que ele consegue processar dados em uma velocidade muito mais alta do que outras aplicações. Na prática, o Redis se torna um banco de dados capaz de desempenhar bem, mesmo com alto volume de informações.

## Como ele funciona

Para ser capaz de funcionar com armazenamento em alta velocidade, o Redis trabalha, basicamente, com dois tipos de processamento:

1. **Armazenamento de valores chaves:**

   O primeiro funciona com a **criação de chaves** para cada entrada de informações no banco de dados. Posteriormente, essas chaves permitem acessar os dados.

   Entre suas características principais, estão a escalabilidade, já que esse esquema de chaves torna a estrutura do banco de dados mais simplificada.
2. **Banco de dados na memória**:

   Já o armazenamento na memória torna a atividade mais rápida, uma vez que esse processamento **leva muito menos tempo do que em outras estruturas tradicionais**, como as que armazenam em discos rígidos.

   O desempenho mais dinâmico pode ser observado tanto em bancos de dados estruturados quanto desestruturados.

## Onde podemos aplicar o Redis em nosso ambiente empresarial

As características do Redis o colocam como um banco de dados que pode ser muito útil em algumas situações específicas, o que reforça sua versatilidade. São atividades comuns a empresas dos mais diversos tipos e que têm necessidades muitas vezes relacionadas a seus respectivos segmentos. Entenda melhor a seguir como essa solução pode ser utilizada.

### Chat e sistema de mensagens

Sua estruturação de processamento de dados em lista é fundamental para que o Redis seja útil no suporte à atividade de chats e sistemas de mensagens que empresas comumente usam. A forma como esse banco de dados funciona, a nível de estruturação de dados, **permite criar filas** de menor porte, ou seja, que serão processadas e terminadas mais rapidamente.

No geral, o Redis será útil em situações como:

* salas de chat;
* caixas de comentários de [live streamings](https://rockcontent.com/br/blog/live-streaming/);
* banco de dados de [chatbots](https://rockcontent.com/br/blog/chatbots/);
* painéis que reproduzam feeds de mídias sociais.

### Streaming de mídia

Atividades de streaming demandam **armazenamento e acesso rápido de dados**, o que ajuda a manter a aplicação capaz de fazer uma transmissão ao vivo. Entre as pequenas tarefas que os streamings executam, às quais o Redis dá o suporte, estão:

* armazenamento de dados de usuários que estão assistindo;
* autenticação dos usuários (geralmente, um grande número de pessoas);
* registro de informações de perfis dos usuários;
* otimizar a comunicação com [CDNs](https://rockcontent.com/br/blog/cdn/) que replicarão a transmissão para um alto volume de pessoas simultaneamente.

### Análise em tempo real

O Redis também é altamente competente para **processar dados em tempo real**, utilizando para isso as mesmas características que o fazem útil para dar suporte a streamings. Um bom exemplo de aplicação são os placares de jogo, muito utilizados por plataformas de apostas e aplicativos de notícias esportivas.

### Machine Learning

O [Machine Learning](https://rockcontent.com/br/blog/machine-learning/) é um campo da tecnologia focado em desenvolver em máquinas a capacidade de aprender com os dados aos quais são expostas. A partir disso, sistemas e softwares passam a entender como replicar essas informações nos momentos certos. Essa é a base para que a [Inteligência Artificial](https://rockcontent.com/br/blog/inteligencia-artificial/) funcione adequadamente em muitas ocasiões.

Como o **volume de informações processados em Machine Learning é grande**, torna-se fundamental ter um banco de dados dinâmico e ágil como o Redis. Essa característica possibilita uma tomada de decisão mais rápida para oferecer respostas a partir do conteúdo que foi recebido pelo sistema.

## Quais os benefícios de utilizar o Redis?

A escolha do Redis para ser banco de dados de aplicações variadas, de [sites](https://rockcontent.com/br/blog/site/) a softwares, pode ser a mais adequada devido a alguns benefícios principais que ele oferece. São vantagens relacionadas às suas características, focadas principalmente em proporcionar dinâmica e rapidez no uso. A seguir, entenda melhor esses fatores e como eles são atrativos.

### Uso dinâmico e fácil

Facilidade de uso é sempre um ponto importante, especialmente quando pensamos em contextos como a rotina de desenvolvimento. O Redis proporciona isso graças ao **baixo nível de código que demanda na hora de gerenciar dados de forma geral**, com processamento e armazenamento, principalmente. Isso o torna mais prático na hora de lidar com as mais variadas aplicações.

Manipular dados é uma tarefa simples no Redis, principalmente porque ele trabalha de forma nativa, ou seja, mantém a estrutura de dados intacta. Assim, todo o trabalho de acesso e captação, muito comuns quando um banco de dados funciona para uma aplicação, fica mais simples e rápido, principalmente.

### Capacidade de replicar e de funcionar de forma recorrente

Replicar dados e comportamentos é essencial quando falamos de bancos de dados. Por isso, o Redis se torna ainda mais relevante, graças à sua facilidade de trabalhar dessa maneira. Esse funcionamento dá **dinamismo à forma como os dados são replicados aos servidores que trabalham de forma associada ao banco de dados**.

Como consequência positiva principal, a leitura de informações se torna muito mais rápida, já que as solicitações são direcionadas para vários servidores, sem que haja lentidão no processamento.

### Escalabilidade

Por conta de sua arquitetura, o Redis permite que as aplicações possam alcançar o nível de performance que desejarem, independentemente do nível de exigência. A qualquer momento, é possível **ajustar o tamanho dos clusters**, aplicando escalabilidade tanto horizontal quanto vertical, adaptando sua infraestrutura de banco de dados às exigências de cada aplicação.

### Suporte a diferentes linguagens

É importante que um banco de dados esteja pronto para processar dados em diferentes [linguagens](https://rockcontent.com/br/blog/linguagem-de-programacao/) e, nesse quesito, o Redis não deixa a desejar. Sua compatibilidade se estende, principalmente, a:

* **[Java](https://rockcontent.com/br/blog/o-que-e-java/);**
* **[Python](https://rockcontent.com/br/blog/python-para-seo/);**
* **[PHP](https://rockcontent.com/br/blog/o-que-e-php/);**
* **C;**
* **C++;**
* **C#;**
* **[JavaScript](https://rockcontent.com/br/blog/javascript/);**
* **[Node.js](https://rockcontent.com/br/blog/node-js/);**
* **Ruby;**
* **R;**
* **Go.**

### **Performance de ponta**

Para que um banco de dados tenha uma performance destacada, é essencial que ele consiga **processar dados em alta velocidade e, acima de tudo, simultaneamente**. O Redis é capaz de entregar isso devido ao fato de que não utiliza armazenamento em disco rígido, nem mesmo SSDs, que são muito mais ágeis. O armazenamento na memória é o grande fator diferencial nesse caso!

### Código aberto

Aplicações de código aberto não são uma novidade e há muito tempo têm sido essenciais para que profissionais do setor possam ter soluções em evolução à sua disposição. O Redis é totalmente **aberto para mudanças por parte de sua comunidade**, o que garante uma estrutura otimizada continuamente, sempre com melhorias que favorecem o usuário.

O Redis é um tipo de banco de dados que pode ser muito útil para aplicações com alta exigências de respostas rápidas e processamento dinâmico. Versátil, ele é capaz de manter um bom nível de desempenho no processamento e gerenciamento de dados, mesmo para as atividades que mais exigem de uma aplicação desse tipo. Em geral, é uma escolha certeira, focada em alto desempenho!

Fonte: [https://rockcontent.com/br/blog/redis/](https://rockcontent.com/br/blog/redis/)

Autor: Ivan de Souza

## Instalação

Para iniciarmos a utilização do banco de dados em memória Redis precisaremos seguir os seguintes passos

1. Primeiramente precisaremos rodar uma imagem do servidor do banco de dados Redis Alpine executando o comando à seguir:

   ```
   docker run --rm -p 6370 --name test-redis redis:6.2-alpine redis-server --loglevel warning
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

4\. Para rodar o Redis com mais opções de configuração a sua instanciação via linha de comando ficará inviável, para isso podemos utilizar um arquivo docker-compose chamado "docker-compose-redis.yml" no qual podemos definir algumas configurações adicionais tais como inclusão de persistência e autenticação:

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
3. Vamos agora explorar alguns exemplos no próprio site do redis no seguinte endereço:

   [https://redis-py.readthedocs.io/en/v4.2.0/examples.html](https://redis-py.readthedocs.io/en/v4.2.0/examples.html):
4. Abordaremos aqui os mais usuais, são eles:

   SET( persistir estruturas simples no banco)

   \

   ```
   r.set('usuario','Marcos')
   # True
   ```

   GET( Recuperar dados do banco de dados)

   ```
   r.get('usuario')
   # Marcos
   ```

   EXISTS ( Verificar se determinada chave existe no banco de dados)

   ```
   r.exists('usuario')
   # Marcos
   ```

   HSET( Para persistirmos e recuperarmos hashsets)

   ```
   r.hset('dados_usuario1', mapping={
   	'nome': 'Jpão',
   	'Sobrenome':'Fernandes',
   	'empresa':'Google'
   	'idade':'32'
   })
   #True

   r.hgetall('dados_usuario')
   # {'nome': 'João', 'Sobrenome':'Fernandes', 'empresa':'Google' 'idade':'32'}
   ```

   MSET(Para persistirmos dicionários com múltiplas chaves)

   ```bash
   dict_data = {
     "employee_name": "Adam Adams",
     "employee_age": 30,
     "position": "Software Engineer",
   }

   r.mset(dict_data)
   ```
5. Ao buscar por múltiplas chaves/valores se a referida chave não existir ou não for passada, Redis retornará “None” para o resultado:

```python
r.mget("employee_name", "employee_age", "position", "non_existing")
#['Adam Adams', '30', 'Software Engineer', None]
```

Vamos verificar na própria documentação do Redis como criar índices e fazer queries:

[https://redis-py.readthedocs.io/en/v4.2.0/examples/search_json_examples.html](https://redis-py.readthedocs.io/en/v4.2.0/examples/search_json_examples.html)

Podemos explorar alguns comandos de manipulação de dados que o Redis nos oferece em sua própria documentação em: [https://redis.io/docs/latest/commands/](https://redis.io/docs/latest/commands/)

## Como podemos integrar o Redis com uma aplicação Flask

Como proposta de uma aplicação exemplo em flask que faz uso das libs python: redis, Flask-Session, e Flask-SQLAlquemy e que comtempla uma aplicação de uma loja com usuários em diferentes filiais que utiliza o conceito de multitenancy para fixarmos os conceitos:

Para tanto teremos as seguintes entidades:

* “User”;
* “Product”;
* “Branch(Filial) e;
* Purchase(Compra)

### Estrutura do Projeto

A estrutura do projeto:

```markup
multi_tenant_app/
│
├── app/
│   ├── __init__.py
│   ├── views.py
│   ├── models.py
│
├── config.py
├── run.py
├── requirements.txt
```

### 1. Arquivo  `requirements.txt`

Adicione SQLAlchemy e Flask-SQLAlchemy às dependências:

```javascript
Flask
Flask-Session
redis
Flask-SQLAlchemy
```

### 2. Configuração do Banco de Dados no `config.py`

```javascript
import os
import redis

class Config:
    SECRET_KEY = os.environ.get('SECRET_KEY') or 'supersecretkey'
    SESSION_TYPE = 'redis'
    SESSION_PERMANENT = False
    SESSION_USE_SIGNER = True
    SESSION_REDIS = redis.from_url('redis://localhost:6379')
    SQLALCHEMY_DATABASE_URI = 'sqlite:///app.db'
    SQLALCHEMY_TRACK_MODIFICATIONS = False
```

### 3. Definição dos Modelos em `app/models.py`

```javascript
from flask_sqlalchemy import SQLAlchemy

db = SQLAlchemy()

class Tenant(db.Model):
    id = db.Column(db.Integer, primary_key=True)
    name = db.Column(db.String(100), nullable=False, unique=True)

class Branch(db.Model):
    id = db.Column(db.Integer, primary_key=True)
    name = db.Column(db.String(100), nullable=False)
    tenant_id = db.Column(db.Integer, db.ForeignKey('tenant.id'), nullable=False)
    tenant = db.relationship('Tenant', backref=db.backref('branches', lazy=True))

class User(db.Model):
    id = db.Column(db.Integer, primary_key=True)
    username = db.Column(db.String(100), nullable=False, unique=True)
    password = db.Column(db.String(100), nullable=False)  # Adicione um campo de senha
    branch_id = db.Column(db.Integer, db.ForeignKey('branch.id'), nullable=False)
    branch = db.relationship('Branch', backref=db.backref('users', lazy=True))

class Product(db.Model):
    id = db.Column(db.Integer, primary_key=True)
    name = db.Column(db.String(100), nullable=False)
    price = db.Column(db.Float, nullable=False)
    branch_id = db.Column(db.Integer, db.ForeignKey('branch.id'), nullable=False)
    branch = db.relationship('Branch', backref=db.backref('products', lazy=True))

class Purchase(db.Model):
    id = db.Column(db.Integer, primary_key=True)
    user_id = db.Column(db.Integer, db.ForeignKey('user.id'), nullable=False)
    product_id = db.Column(db.Integer, db.ForeignKey('product.id'), nullable=False)
    quantity = db.Column(db.Integer, nullable=False)
    user = db.relationship('User', backref=db.backref('purchases', lazy=True))
    product = db.relationship('Product', backref=db.backref('purchases', lazy=True))
```

### 4. Vamos criar o arquivo `app/__init__.py`com o seguinte conteúdo

```markup
from flask import Flask
from flask_session import Session
from flask_sqlalchemy import SQLAlchemy
import redis

db = SQLAlchemy()

def create_app():
    app = Flask(__name__)
    app.config.from_object('config.Config')

    # Initialize extensions
    Session(app)
    db.init_app(app)

    with app.app_context():
        from . import views, models
        db.create_all()
        app.register_blueprint(views.bp)

    return app
```

5. Arquivo "run.py"

   ```
   from app import create_app

   app = create_app()

   if __name__ == '__main__':
       app.run(debug=True)

   ```

6. **Rotas e Lógica de Login:**

Adicione uma rota para login e armazene a filial do usuário na sessão.

```python
return jsonify(message="Tenants registered", tenants=created_tenants)

@bp.route('/register_user', methods=['POST'])
def register_user():
    data = request.json
    username = data.get('username')
    password = data.get('password')
    branch_id = data.get('branch_id')
  
    branch = Branch.query.get_or_404(branch_id)
  
    user = User(username=username, password=generate_password_hash(password), branch_id=branch_id)
    db.session.add(user)
    db.session.commit()
  
    return jsonify(message="User registered", user_id=user.id)

@bp.route('/login', methods=['POST'])
def login():
    data = request.json
    username = data.get('username')
    password = data.get('password')

    user = User.query.filter_by(username=username).first()
    if user and check_password_hash(user.password, password):
        session['user_id'] = user.id
        session['branch_id'] = user.branch_id
        return jsonify(message="Login successful")
    return jsonify(error="Invalid credentials"), 401

@bp.route('/products')
def get_products():
    branch_id = session.get('branch_id')
    if not branch_id:
        return jsonify(error="User not logged in"), 401

    products = Product.query.filter_by(branch_id=branch_id).all()
    return jsonify(products=[{"id": p.id, "name": p.name, "price": p.price} for p in products])

@bp.route('/purchase', methods=['POST'])
def create_purchase():
    branch_id = session.get('branch_id')
    if not branch_id:
        return jsonify(error="User not logged in"), 401

    data = request.json
    user_id = session.get('user_id')
    product_id = data.get('product_id')
    quantity = data.get('quantity')
  
    user = User.query.get_or_404(user_id)
    product = Product.query.get_or_404(product_id)
  
    if product.branch_id != branch_id:
        return jsonify(error="Unauthorized access"), 403
  
    purchase = Purchase(user_id=user_id, product_id=product_id, quantity=quantity)
    db.session.add(purchase)
    db.session.commit()
  
    return jsonify(message="Purchase created", purchase_id=purchase.id)
```

### Execução da aplicação

Instale as dependências:

`pip install -r requirements.txt`

Em seguida execute a aplicação:

```
python run.py
```

### Explicação

1. **Configuração da Sessão com Redis**: A configuração no `create_app` define a sessão para utilizar Redis como backend, armazenando as sessões no banco de dados Redis.
2. **Rota** `/login`: Autentica o usuário, armazena o `user_id` e `branch_id` na sessão após o login.
3. **Rota** `/products`: Consulta os produtos filtrando pela `branch_id` armazenada na sessão.
4. **Rota** `/purchase`: Cria uma compra, garantindo que o usuário só pode comprar produtos da sua filial.

### Teste Completo

1. **Registrar Múltiplos Tenants**:

   ```markup
   curl -X POST http://127.0.0.1:5000/register_tenants -H "Content-Type: application/json" -d '{"tenant_names": ["tenant1", "tenant2"]}'
   ```
2. **Registrar um Usuário**:

   ```markup
   curl -X POST http://127.0.0.1:5000/register_user -H "Content-Type: application/json" -d '{"username": "newuser", "password": "password123", "branch_id": 1}'
   ```
3. **Login do Usuário**:

   ```javascript
   curl -X POST http://127.0.0.1:5000/login -H "Content-Type: application/json" -d '{"username": "newuser", "password": "password123"}'
   ```
4. **Consultar Produtos da Filial do Usuário**:

   ```javascript
   curl -X GET http://127.0.0.1:5000/products
   ```

Essa abordagem garante que, após o login, as requisições subsequentes do usuário estarão restritas aos produtos e operações relacionadas à sua filial, utilizando a sessão armazenada no Redis para persistência dos dados de sessão.

Referências:

[https://redis.io/docs/](https://redis.io/docs/)

[https://geshan.com.np/blog/2022/01/redis-docker/](https://geshan.com.np/blog/2022/01/redis-docker/)

[https://rockcontent.com/br/blog/redis/](https://rockcontent.com/br/blog/redis/)

[https://redis-py.readthedocs.io/en/v4.2.0/redismodules.html](https://redis-py.readthedocs.io/en/v4.2.0/redismodules.html)
