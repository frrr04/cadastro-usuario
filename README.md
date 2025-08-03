# Cadastro de Usuário

Este é um projeto backend desenvolvido com Spring Boot, que fornece uma API REST para gerenciamento de usuários. A aplicação permite realizar operações básicas como criação, listagem, atualização e exclusão de registros de usuário.

## Tecnologias Utilizadas

- Java 24
- Spring Boot
- Spring Data JPA
- Maven
- H2 Database (padrão para testes)
- Lombok

## Estrutura do Projeto

- `controller`: expõe os endpoints REST da API
- `business`: contém a lógica de negócio da aplicação
- `infrastructure/entitys`: define a entidade `Usuario`
- `infrastructure/repository`: interface com o banco de dados via Spring Data JPA

## Requisitos

- Java 17 ou superior
- Maven 3.8 ou superior

## Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/frrr04/cadastro-usuario.git
   ```

2. Acesse o diretório do projeto:
   ```bash
   cd cadastro-usuario
   ```

3. Compile e execute a aplicação:
   ```bash
   ./mvnw spring-boot:run
   ```

4. A aplicação estará disponível em:
   ```
   http://localhost:8080
   ```

## Banco de Dados

Por padrão, a aplicação utiliza o banco H2 em memória. Os dados são reiniciados a cada execução.

## Observações

- O projeto utiliza Lombok. Certifique-se de que seu IDE está com o plugin do Lombok instalado e habilitado.
- As configurações podem ser ajustadas no arquivo `src/main/resources/application.properties`.
