# TypeORM

O **TypeORM** é uma biblioteca de ORM (Object-Relational Mapping) escrita em TypeScript e JavaScript, que permite as desenvolvedoras trabalhar com bancos de dados relacionais de forma mais orientada a objetos. Ele fornece uma camada de abstração entre o código da aplicação e o banco de dados, permitindo que as desenvolvedoras interajam com o banco de dados usando objetos e classes em vez de escrever consultas SQL diretamente.

O TypeORM simplifica o processo de mapeamento de entidades de aplicação para tabelas de banco de dados, gerenciando automaticamente operações como criação, leitura, atualização e exclusão (CRUD), bem como relacionamentos entre entidades.

Quando falamos de "TypeORM com PostgreSQL", estamos nos referindo ao uso específico do TypeORM para interagir com um banco de dados PostgreSQL. Isso significa que estamos aproveitando as funcionalidades do TypeORM para mapear nossas entidades TypeScript/JavaScript para tabelas PostgreSQL, bem como executar operações CRUD e consultas usando a sintaxe oferecida pelo TypeORM, em vez de escrever SQL manualmente.

É importante entender os conceitos subjacentes ao TypeORM, como entidades, repositórios, relacionamentos, consultas e migrações. Dominar esses comandos e conceitos permitirá que você utilize o TypeORM de forma eficaz em seus projetos, especialmente quando combinado com PostgreSQL.

## 👉 Instalação do TypeORM

Para executar comandos do TypeORM precisamos fazer a instalação da ferramenta globalmente:

```sh
npm install -g typeorm
```

## 👉 Comandos utilizados

1. **typeorm init**: Este comando é usado para inicializar um novo projeto TypeORM. Ele cria a estrutura básica de arquivos e pastas necessários para começar a trabalhar com o TypeORM em seu projeto.
2. **typeorm migration:create**: Usado para criar uma nova migração. As migrações são arquivos que descrevem as alterações no esquema do banco de dados. Este comando cria um novo arquivo de migração com um nome significativo.
3. **typeorm migration:generate**: Gera uma nova migração automaticamente com base nas diferenças detectadas entre o esquema atual do banco de dados e o esquema definido pelas entidades TypeORM em seu projeto.
4. **typeorm migration:run**: Executa todas as migrações pendentes para atualizar o esquema do banco de dados de acordo com as alterações definidas nas migrações.
5. **typeorm migration:revert**: Reverte a última migração aplicada, desfazendo as alterações feitas no esquema do banco de dados.
6. **typeorm entity:create**: Cria uma nova entidade (tabela) TypeORM. Este comando cria um novo arquivo de classe TypeScript que representa uma entidade no seu projeto.
7. **typeorm entity:sync**: Sincroniza automaticamente o esquema do banco de dados com as entidades definidas em seu projeto. Este comando cria ou altera tabelas de banco de dados com base nas entidades TypeORM no seu projeto.
8. **typeorm query**: Executa uma consulta SQL direta usando o TypeORM.
