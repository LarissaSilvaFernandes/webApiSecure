# Projeto Spring Security

Este projeto é um estudo de Spring Boot com Spring Security, utilizando uma arquitetura MVC e integração com MongoDB para autenticação e autorização de usuários.

## Tecnologias Utilizadas

- Java 8
- Spring Boot 2.5.5
- Spring Security
- Spring Data JPA
- Spring Data MongoDB
- H2 Database (para testes)
- Maven

## Estrutura do Projeto

- `WelcomeController`: Controlador para endpoints de boas-vindas e autorização.
- `SecurityDatabaseService`: Serviço que carrega os detalhes do usuário a partir do banco de dados.
- `WebSecurityConfig`: Configuração de segurança da aplicação.
- `StartApplication`: Classe para inicializar o banco de dados com usuários padrão.
- `User`: Entidade representando o usuário.
- `UserRepository`: Repositório para a entidade `User`.

## Endpoints
- GET /: Endpoint público que retorna uma mensagem de boas-vindas.
- GET /users: Endpoint protegido que retorna uma mensagem para usuários autorizados.
- GET /managers: Endpoint protegido que retorna uma mensagem para gerentes autorizados.

## Executando o Projeto

Para executar o projeto, utilize o seguinte comando:

```sh
mvn spring-boot:run
  A aplicação estará disponível em http://localhost:8080.
  ```

## Licença
Este projeto está licenciado sob os termos da licença MIT. Veja o arquivo LICENSE para mais detalhes.