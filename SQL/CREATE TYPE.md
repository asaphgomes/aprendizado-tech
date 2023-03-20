# CRIAR TIPO

O comando **CREATE TYPE** é usado para criar um novo tipo de dados definido pelo usuário no banco de dados. Esses tipos de dados personalizados podem ser usados para criar colunas personalizadas em tabelas de banco de dados.

**DOCUMENTAÇÃO:** https://www.postgresql.org/docs/current/sql-createtype.html

## Sintaxe

A sintaxe básica para criar um novo tipo de dados é a seguinte:

```sql
CREATE TYPE nome_do_tipo AS (definição_do_tipo);
```

Onde:

- **nome_do_tipo**: é o nome do novo tipo de dados a ser criado.
- **definição_do_tipo**: é a estrutura de dados definida pelo usuário que define o novo tipo de dados.

A definição do tipo pode incluir vários tipos de dados pré-definidos e outros tipos de dados definidos pelo usuário. Por exemplo, se quisermos criar um novo tipo de dados que represente um endereço, podemos definir a estrutura de dados da seguinte forma:

```sql
CREATE TYPE endereco AS (
    rua varchar(50),
    cidade varchar(50),
    estado char(2),
    cep char(8)
);
```

Agora, podemos usar o tipo de dados personalizado **endereco** para criar uma nova tabela com uma coluna personalizada do tipo **endereco**:

```sql
CREATE TABLE clientes (
    id int,
    nome varchar(50),
    endereco endereco
);
```

O comando **CREATE TYPE** é uma ferramenta poderosa para criar tipos de dados personalizados em um banco de dados. Isso permite que os usuários criem estruturas de dados altamente personalizadas e reutilizáveis, tornando o processo de modelagem de dados mais eficiente e flexível.
