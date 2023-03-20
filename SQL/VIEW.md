# VIEW

Em SQL, uma View é uma tabela virtual que mostra um resultado determinado de uma consulta SQL. Ela contém linhas e colunas, como uma tabela normal. Os campos da View são campos de uma ou mais tabelas reais do banco de dados. Você pode adicionar funções e comandos para uma View e mostrar os dados como se eles viessem de uma única tabela. Seria como se fosse uma variável que armazena a consulta SQL que define a View.

Existem dois tipos de Views: Views atualizáveis e Views não atualizáveis.

- As Views atualizáveis permitem a execução de operações DML nos dados da View, de forma que sejam atualizados, inseridos ou excluídos. Para criar uma View atualizável, ela deve atender a certos requisitos, como ter uma única tabela base, não conter funções agregadas, DISTINCT ou UNION, entre outros.
- As Views não atualizáveis, por outro lado, não permitem que os dados da View sejam atualizados, inseridos ou excluídos. Isso pode ser útil em casos onde os dados da View são usados apenas para consulta e análise, sem a necessidade de modificá-los. Além disso, Views não atualizáveis têm melhor desempenho do que Views atualizáveis, pois não precisam lidar com a lógica de atualização de dados.

Para criar uma View, use a sintaxe `CREATE VIEW`. A seguir, um exemplo:

```sql
CREATE VIEW vw_name AS SELECT column_1, column_2... FROM table_name WHERE condition
```

- `REPLACE VIEW`: substitui a definição de uma View existente por uma nova definição. A sintaxe é:

```sql
REPLACE VIEW vw_name AS SELECT column_1, column_2... FROM table_name WHERE condition;
```

- `DROP VIEW`: exclui uma View existente. A sintaxe é:

```sql
DROP VIEW vw_name;
```
Lembre-se de que, ao excluir uma View, todos os dados contidos nela também serão excluídos.

OBS: Recomenda-se utilizar 'vw_' como prefixo para o nome da View para identificá-la.
