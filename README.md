# proj-recup

### Contextualização:
Você foi contratado como desenvolvedor para criar um sistema de cadastro de livros para uma biblioteca local. O sistema será acessado por bibliotecários que precisam registrar novos livros na base de dados, atualizar informações sobre os livros existentes, consultar os livros cadastrados e excluir livros quando necessário.

A biblioteca deseja ter um controle eficiente sobre os livros disponíveis, incluindo informações como título, autor, gênero, ano de publicação e quantidade de exemplares. Para isso, você deverá construir uma aplicação web utilizando Python, Flask para o backend e MySQL como banco de dados.

### Requisitos Funcionais:

**Cadastro de Livros:**

O sistema deve permitir o cadastro de novos livros, com os seguintes campos obrigatórios:

- Título: Nome do livro.

- Autor: Nome do autor do livro.

- Gênero: Gênero literário do livro (ex: Ficção, História, Ciência, etc.).

- Ano de publicação: Ano em que o livro foi publicado.

- Quantidade de exemplares: Número de cópias disponíveis do livro na biblioteca.

**Persistência de Dados:**

O sistema deve utilizar um banco de dados MySQL para armazenar as informações sobre os livros.

A tabela livros deve conter os seguintes campos:

- id (INT, chave primária, autoincremento)

- titulo (VARCHAR)

- autor (VARCHAR)

- genero (VARCHAR)

- ano_publicacao (INT)

- quantidade_exemplares (INT)

**Interface Web:**

- O sistema deve ter uma interface web simples para interagir com os usuários. Você deve criar:

  - Formulário de cadastro de livros.

- A interface será desenvolvida utilizando o **Flask**.

  ### Exemplo de Estrutura de Banco de Dados (MySQL):

```
CREATE DATABASE biblioteca;

USE biblioteca;

CREATE TABLE livros (
    id INT AUTO_INCREMENT PRIMARY KEY,
    titulo VARCHAR(255) NOT NULL,
    autor VARCHAR(255) NOT NULL,
    genero VARCHAR(100),
    ano_publicacao INT,
    quantidade_exemplares INT
);

```

