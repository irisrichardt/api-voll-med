# API Voll Med

Esta é uma API RESTful desenvolvida em Java com o framework Spring Boot. O projeto foi criado durante um curso, com o objetivo de aprender e implementar uma API completa para a gestão de dados médicos, incluindo operações de CRUD, paginação de dados e validações.

## Funcionalidades

- **CRUD Completo**: Gerenciamento de recursos, permitindo a criação, leitura, atualização e exclusão de dados médicos no banco de dados.
- **Banco de Dados MySQL**: Integração com o MySQL para armazenamento persistente dos dados.
- **Migrations com Flyway**: Utilização do Flyway para controle de versões e migrações do banco de dados, permitindo a atualização e estruturação das tabelas de forma consistente.
- **Validações com Bean Validation**: Validação de dados de entrada, garantindo a integridade das informações enviadas para a API.
- **Paginação e Ordenação**: Implementação de paginação para exibição organizada e eficiente dos dados.

## Tecnologias Utilizadas

- **Java**: Linguagem de programação principal.
- **Spring Boot**: Framework para desenvolvimento rápido de aplicações Java.
- **MySQL**: Banco de dados relacional para armazenamento dos dados.
- **Flyway**: Ferramenta de migração de banco de dados.
- **Bean Validation**: Framework para validação de dados.
- **Spring Data JPA**: Abstração de acesso a dados que facilita a implementação de operações com o banco de dados.

## Como Executar o Projeto

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/irisrichardt/api-voll-med.git
   cd api-voll-med
   ```

2. **Configure o Banco de Dados**:
    - Certifique-se de ter o MySQL instalado e em execução.
    - Crie um banco de dados para o projeto.
    - No arquivo `application.properties`, configure as informações de conexão com o banco de dados:
      ```properties
      spring.datasource.url=jdbc:mysql://localhost:3306/nome_do_banco
      spring.datasource.username=seu_usuario
      spring.datasource.password=sua_senha
      ```

## Endpoints da API

Exemplo de alguns dos endpoints disponíveis:

- `GET /medicos` - Lista todos os médicos com suporte a paginação.
- `POST /medicos` - Cria um novo registro de médico.
- `GET /medicos/{id}` - Busca os dados de um médico específico.
- `PUT /medicos/{id}` - Atualiza as informações de um médico.
- `DELETE /medicos/{id}` - Remove o registro de um médico.
