# Projeto: Gerenciamento de Tarefas

## Objetivo

Construir uma aplicação web no modelo MVC para o gerenciamento de tarefas com persistência de dados em H2, MariaDB e MongoDB.

## Tecnologias Utilizadas

- Java 17
- Spring Boot
- Spring Data JPA
- Spring Data MongoDB
- Lombok
- H2 Database
- MariaDB
- Maven

## Executando o Projeto

1. Importe o projeto no Visual Studio Code ou outra IDE de sua preferência.
2. Certifique-se de ter o Java 17 instalado.
3. Execute a classe `TarefasApplication`.
4. Use o Postman ou outro cliente HTTP para testar os endpoints em `http://localhost:8080/tarefas`.

## Endpoints

- `GET /tarefas` – Lista todas as tarefas.
- `POST /tarefas` – Cria uma nova tarefa.
- `PUT /tarefas/{id}` – Atualiza uma tarefa existente.
- `DELETE /tarefas/{id}` – Exclui uma tarefa.

## Banco de Dados

- O projeto está configurado para usar o banco H2 por padrão.
- Para usar MariaDB ou MongoDB, descomente as configurações em `application.properties`.

## Autor

Projeto acadêmico desenvolvido com fins educacionais.
