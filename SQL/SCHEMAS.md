# SCHEMAS

Um schema em SQL é uma coleção lógica de objetos de banco de dados, como tabelas, visualizações, procedimentos armazenados, etc. Os objetos são geralmente relacionados a um aplicativo específico ou a um usuário específico.

Os schemas podem ser usados para separar objetos de banco de dados pertencentes a aplicativos diferentes, evitando conflitos de nomeação de objetos. Eles também podem ajudar a gerenciar a segurança e as permissões de acesso aos objetos de banco de dados.

Para criar um novo schema em um banco de dados, você pode usar o comando CREATE SCHEMA. Por exemplo, para criar um schema chamado "meuschema", você pode usar o seguinte comando:

```sql
CREATE SCHEMA meuschema;
```

Depois de criar um schema, você pode criar objetos de banco de dados dentro dele, como tabelas e procedimentos armazenados. Para fazer isso, você precisa especificar o nome do schema antes do nome do objeto. Por exemplo, para criar uma tabela chamada "minhatabela" dentro do schema "meuschema", você pode usar o seguinte comando:

```sql
CREATE TABLE meuschema.minhatabela (coluna1 tipo1, coluna2 tipo2, ...);
```

Para acessar objetos de banco de dados dentro de um schema, você precisa especificar o nome do schema antes do nome do objeto. Por exemplo, para selecionar todos os registros da tabela "minhatabela" dentro do schema "meuschema", você pode usar o seguinte comando:

```sql
SELECT * FROM meuschema.minhatabela;
```

Em resumo, schemas podem ajudar a organizar e gerenciar objetos de banco de dados em um aplicativo ou em um ambiente de múltiplos usuários.
