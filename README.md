# 📦 Produtos API
 
 ## 📝 Descrição
 A **Produtos API** é uma API RESTful desenvolvida em **Java Spring Boot** para gerenciar um catálogo de produtos.
 
 Ela permite:
 - Criar, atualizar, listar e deletar produtos.
 - Buscar produtos pelo nome ou categoria.
 - Testar requisições via **Postman**.
 
 ## 🚀 Tecnologias Utilizadas
 - **Java 17**
 - **Spring Boot**
 - **Spring Data JPA** (para interação com o banco de dados)
 - **Spring Web** (para criar a API REST)
 - **PostgreSQL** (banco de dados)
 - **Swagger** (documentação da API)
 - **Lombok** (para reduzir boilerplate code)
 - **Postman** (para testes das requisições HTTP)
 
 ## ⚙️ Como Configurar e Executar o Projeto
 ### 🔹 Pré-requisitos
 Certifique-se de ter instalado:
 - [Java 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)
 - [Maven](https://maven.apache.org/)
 - [PostgreSQL](https://www.postgresql.org/download/)
 - [IntelliJ IDEA](https://www.jetbrains.com/idea/download/) ou [Eclipse](https://www.eclipse.org/downloads/)
 
 ### 🔹 Clonar o Repositório
 ```sh
 git clone https://github.com/seuusuario/produtosapi.git
 cd produtosapi
 ```
 
 ### 🔹 Configurar o Banco de Dados
 No PostgreSQL, crie um banco de dados chamado **produtos_db** e configure as credenciais no arquivo `application.properties`:
 ```properties
 spring.datasource.url=jdbc:postgresql://localhost:5432/produtos_db
 spring.datasource.username=seu_usuario
 spring.datasource.password=sua_senha
 ```
 
 ### 🔹 Executar o Projeto
 No terminal, dentro da pasta do projeto, rode:
 ```sh
 mvn spring-boot:run
 ```
 A API estará disponível em: `http://localhost:8080`
 
 ## 📌 Endpoints da API
 | Método  | Endpoint           | Descrição |
 |---------|-------------------|-----------|
 | `GET`   | `/produtos`       | Lista todos os produtos |
 | `GET`   | `/produtos/{id}`  | Busca um produto pelo ID |
 | `POST`  | `/produtos`       | Cadastra um novo produto |
 | `PUT`   | `/produtos/{id}`  | Atualiza um produto existente |
 | `DELETE`| `/produtos/{id}`  | Remove um produto |
 
 ### 🔹 Testando no Postman
 Após iniciar o projeto, abra o **Postman** e envie requisições para `http://localhost:8080/produtos` conforme os métodos acima.
 
 ## 📚 Documentação com Swagger
 A documentação interativa da API pode ser acessada após rodar o projeto em:
 ```
 http://localhost:8080/swagger-ui.html
 ```
 
 ## 👨‍💻 Autora
 Desenvolvido por **Vitória Santos Almeida** 🚀
 
 ---
 
