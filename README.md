## Endpoints:

- **Patrimônio:**

GET patrimonios - Obter todos os patrimônios

GET patrimonios/{id} - Obter um patrimônio por ID

POST patrimonios - Inserir um novo patrimônio

PUT patrimonios/{id} - Alterar os dados de um patrimônio

DELETE patrimonios/{id} - Excluir um patrimônio

- **Marcas:**

GET marcas/{id} - Obter uma marca por ID

GET marcas - Obter todas as marcas

GET marcas/{id}/patrimônios - Obter todos os patrimônios de uma marca

POST marcas - Inserir uma nova marca

PUT marca/{id} - Alterar os dados de uma marca

DELETE marca/{id} - Excluir uma marca

- **Usuários:**

GET usuarios – Listar os usuários

POST usuarios – Criar um usuário

Exemplo:

     {
        "id": "2",
        "nome": "gabriel",
        "email": "gabriel@test.com",
        "senha": "pword"
    }

DELETE usuários/{id} – Excluir um usuário

## Autenticação:

- **URL:**
  http://localhost:8080/login

- **Body:**
  {
  "username" : "admin",
  "password" : "password"
  }

Tipo do token gerado:

- **Authorization Type:** Bearer Token

## Banco de dados:

- **SGBD:** PostgreSQL
- **script:** /empresa/script/bancoEmpresa.sql

### Requisitos

- Java 8
- Maven

### Executar

Na raiz do projeto, executar da seguinte forma:

`mvn spring-boot:run`
