# Sistema de Gerenciamento de Clientes - Padoca do Joca

Um sistema integrado para gerenciamento de clientes, endereços e operações relacionadas, utilizando JavaFX e padrão DAO para conexão com bancos de dados.

## Funcionalidades Principais

- **CRUD de Clientes**:
  - Cadastro, consulta, atualização e exclusão de clientes.
  - Vinculação automática de endereços via CEP.
- **Gerenciamento de Endereços**:
  - Busca de endereços por CEP.
- **Módulos Adicionais**:
  - Pedidos, consultas e funcionários (implementação baseada em botões no menu).

## Tecnologias Utilizadas

- **Linguagem**: Java 11
- **Interface Gráfica**: JavaFX 13
- **Gerenciamento de Dependências**: Maven
- **Banco de Dados**:
  - MySQL (`mysql-connector-java 8.0.31`)
  - MariaDB (`mariadb-java-client 3.0.9`)
  - SQL Server (`mssql-jdbc 9.4.0.jre11`)
- **Padrão de Projeto**: DAO (Data Access Object)

## Pré-requisitos

- JDK 11 ou superior
- Maven 3.8.0+
- Banco de dados configurado (MySQL, MariaDB ou SQL Server)

## Configuração e Execução

### Clonar o Repositório
```bash
git clone https://github.com/seu-usuario/Padoca_do_Joca.git
cd Padoca_do_Joca

// Exemplo de conexão (ajuste URL, usuário e senha)
Connection conexao = DriverManager.getConnection(
    "jdbc:mysql://localhost:3306/nome_banco", 
    "usuario", 
    "senha"
);

mvn clean javafx:run

Observação: Certifique-se de configurar corretamente as dependências do banco de dados no pom.xml de acordo com o SGBD utilizado.
