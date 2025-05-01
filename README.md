# 📝 Projeto de Gerenciamento de Tarefas (Modelo MVC)

Este é um projeto acadêmico desenvolvido com **Spring Boot** no padrão arquitetural **MVC (Model-View-Controller)**, que tem como objetivo realizar o **gerenciamento de tarefas**, com persistência de dados em **H2**, **MariaDB** e **MongoDB**.

---

## 🚀 Tecnologias Utilizadas

- Java 17  
- Spring Boot 3.x  
- Spring Web  
- Spring Data JPA  
- Spring Data MongoDB  
- Lombok  
- H2 Database  
- MariaDB  
- MongoDB  
- Maven  
- VS Code  

---

## 📁 Estrutura do Projeto

src/ └── main/ └── java/ └── com.exemplo.tarefas/ ├── controller/ ├── model/ ├── repository/ └── service/


- **Model:** Representa a entidade `Tarefa`  
- **Repository:** Interfaces JPA e MongoRepository para persistência  
- **Service:** Lógica de negócio  
- **Controller:** Endpoints REST  

---

## 🧩 Entidade Principal

java
public class Tarefa {
    private Long id;
    private String titulo;
    private String descricao;
    private String status;
    private LocalDateTime dataCriacao;
}

🔧 Configuração de Banco de Dados

As configurações são feitas no arquivo application.properties.

H2 (Memória):

spring.datasource.url=jdbc:h2:mem:tarefasdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.h2.console.enabled=true

MariaDB:

spring.datasource.url=jdbc:mariadb://localhost:3306/tarefas
spring.datasource.username=root
spring.datasource.password=senha
spring.jpa.hibernate.ddl-auto=update
spring.jpa.database-platform=org.hibernate.dialect.MariaDBDialect

MongoDB:

spring.data.mongodb.uri=mongodb://localhost:27017/tarefasdb

📫 Endpoints REST

GET /tarefas → Lista todas as tarefas

GET /tarefas/{id} → Consulta uma tarefa por ID

POST /tarefas → Cria uma nova tarefa

PUT /tarefas/{id} → Atualiza uma tarefa existente

DELETE /tarefas/{id} → Exclui uma tarefa

✅ Como Executar

Clone o repositório:

git clone https://github.com/seu-usuario/seu-repositorio.git

Acesse a pasta do projeto:

cd seu-repositorio

Execute com Maven:

./mvnw spring-boot:run

🛠️ Requisitos

✅ JDK 17 instalado

✅ Lombok configurado na IDE

✅ MongoDB ou MariaDB em execução (caso não utilize H2)

🧪 Testes

Use ferramentas como Postman ou Insomnia para testar os endpoints da API.

👨‍🎓 Autor

Desenvolvido por Lorrane Maria
Trabalho acadêmico da disciplina Arquitetura de Aplicações Web
Newton Paiva - 2025

