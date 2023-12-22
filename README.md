# Implementando um Banco de Dados Relacional com SQLAlchemy

Nesta parte do projeto, desenvolvemos uma aplicação de integração com SQLite utilizando a biblioteca SQLAlchemy. O objetivo é criar um banco de dados relacional com base em um esquema disponibilizado, focando nos conceitos de cliente e conta.

## Definindo as Tabelas e Relacionamentos:

Criamos duas classes, Cliente e Conta, que representam as tabelas do banco de dados relacional.
Cliente possui campos como id, nome, email e telefone.
Conta inclui campos como id, numero, saldo e uma chave estrangeira cliente_id referenciando a tabela Cliente.
Estabelecemos um relacionamento bidirecional entre as tabelas utilizando a função relationship do SQLAlchemy.
Operações no Banco de Dados:

## Implementamos funções para criar o banco de dados, inserir dados mínimos e recuperar informações utilizando SQLAlchemy.
A função criar_banco_dados() utiliza a função create_all() para criar as tabelas no banco de dados SQLite.
Inserção de Dados Mínimos:

Utilizamos a função inserir_dados(session) para adicionar registros nas tabelas Cliente e Conta.
Exemplificamos a criação de clientes (Rafael, Elaine e Stephanie) e suas respectivas contas.
Recuperação de Dados:

Implementamos a função recuperar_dados(session) para realizar consultas utilizando SQLAlchemy.
Exemplificamos consultas para recuperar todos os clientes e contas, bem como contas com saldo maior que 500.
Conexão com o Banco de Dados:

Criamos uma sessão do SQLAlchemy para interagir com o banco de dados SQLite.
Executando o Projeto:
Instalação de Dependências:

Instale as bibliotecas necessárias utilizando pip install -r requirements.txt.
Criando o Banco de Dados:

Execute criar_banco_dados() para criar as tabelas no banco de dados.
Inserindo Dados:

Execute inserir_dados(session) para adicionar dados mínimos às tabelas.
Recuperando e Exibindo Dados:

Execute recuperar_dados(session) para realizar consultas e visualizar os resultados.

Este conjunto de operações proporciona uma visão geral da implementação do banco de dados relacional com SQLAlchemy, permitindo a manipulação e recuperação eficientes de informações. Certifique-se de seguir as instruções acima para experimentar a aplicação.
