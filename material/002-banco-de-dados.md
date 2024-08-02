# Banco de Dados

## O que é um Banco de Dados?

Um banco de dados é uma coleção organizada de dados que são estruturados de forma que possam ser facilmente acessados, gerenciados e atualizados.

- Comparação com uma planilha ou arquivo de texto: Enquanto uma planilha ou arquivo de texto pode armazenar dados, um banco de dados oferece uma estrutura mais robusta e organizada para lidar com grandes volumes de informações.

## Por que usamos Bancos de Dados?

- Eficiência no armazenamento e recuperação de dados.
- Consistência e integridade dos dados.
- Suporte a múltiplos usuários e aplicativos.
- Segurança dos dados.
- Escalabilidade para lidar com grandes quantidades de dados.

## Componentes de um Banco de Dados

- **Dados**: São as informações armazenadas no banco de dados.
- **Sistema de Gerenciamento de Banco de Dados (SGBD)**: É o software responsável por gerenciar o banco de dados. Exemplos populares incluem MySQL, PostgreSQL, Oracle, SQL Server, entre outros.
- **Usuários**: São as pessoas ou aplicativos que interagem com o banco de dados.
- **Modelo de Dados**: Define a estrutura dos dados e como eles estão organizados no banco de dados. Exemplos incluem modelos relacionais, orientados a documentos, entre outros.
- **Linguagem de Consulta**: É a linguagem usada para interagir com o banco de dados e realizar operações como inserção, consulta, atualização e exclusão de dados. Exemplos incluem SQL (Structured Query Language) e NoSQL Query Languages.

##Tipos de Bancos de Dados

- **Bancos de Dados Relacionais**: Organizam os dados em tabelas relacionadas umas com as outras por meio de chaves primárias e estrangeiras. Exemplos incluem MySQL, PostgreSQL, SQL Server.
- **Bancos de Dados NoSQL**: São bancos de dados que não seguem o modelo relacional tradicional. Eles são projetados para lidar com grandes volumes de dados não estruturados ou semiestruturados. Exemplos incluem MongoDB, Cassandra, Redis.

## Operações Básicas em Banco de Dados

- **CRUD**: Create (Criação), Read (Leitura), Update (Atualização), Delete (Exclusão).
- Exemplos de consultas SQL básicas para realizar cada operação.

## ORM (Object-Relational Mapping)

- Definição básica: ORM é uma técnica de programação que mapeia objetos de um sistema orientado a objetos para tabelas em um banco de dados relacional.
- Objetivo: Simplificar o processo de interação entre o código da aplicação e o banco de dados, abstraindo as complexidades do SQL e permitindo que os desenvolvedores trabalhem com objetos em vez de consultas SQL diretamente.
- Vantagens:
  - Redução da quantidade de código SQL manual necessário.
  - Maior produtividade no desenvolvimento de aplicativos.
  - Melhor legibilidade e manutenção do código.
  - Facilita a portabilidade entre diferentes sistemas de banco de dados.
- Exemplos de ORM populares: Hibernate (para Java), Entity Framework (para .NET), Django ORM (para Python), Sequelize (para Node.js).

## Como funciona o ORM

- **Mapeamento Objeto-Relacional (ORM Mapping)**: É o processo de definir como os objetos da aplicação estão relacionados com as tabelas do banco de dados.
- **Entidades (Entities)**: São as classes de objetos que representam tabelas no banco de dados.
- **Atributos (Attributes)**: São as propriedades das entidades que correspondem às colunas das tabelas.
- **Relacionamentos (Relationships)**: São as associações entre diferentes entidades que refletem as relações entre tabelas no banco de dados (por exemplo, um-para-muitos, muitos-para-muitos).
- **Operações CRUD com ORM**: As operações básicas de criar, ler, atualizar e excluir são realizadas por meio de métodos específicos fornecidos pelo ORM, sem a necessidade de escrever consultas SQL manualmente.
