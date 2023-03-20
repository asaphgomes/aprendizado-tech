# Métricas de Agregação em SQL

As métricas de agregação em SQL são funções utilizadas para realizar cálculos em conjunto de dados agrupados. Estas funções podem ser aplicadas em conjunto com a cláusula "GROUP BY" para fornecer resultados agregados para cada grupo de dados.

As métricas de agregação mais comuns são:

## COUNT

A métrica COUNT é utilizada para contar o número de linhas em uma tabela ou grupo de dados. Sua sintaxe com e sem GROUP BY é:

```sql
SELECT COUNT(column_name) FROM table_name;
SELECT column_name, COUNT(column_name) FROM table_name GROUP BY column_name;
```

## SUM

A métrica SUM é utilizada para somar os valores de uma coluna ou grupo de dados. Sua sintaxe com e sem GROUP BY é:

```sql
SELECT SUM(column_name) FROM table_name;
SELECT column_name, SUM(column_name) FROM table_name GROUP BY column_name;
```

## AVG

A métrica AVG é utilizada para calcular a média dos valores de uma coluna ou grupo de dados. Sua sintaxe com e sem GROUP BY é:

```sql
SELECT AVG(column_name) FROM table_name;
SELECT column_name, AVG(column_name) FROM table_name GROUP BY column_name;

```

## MAX

A métrica MAX é utilizada para encontrar o valor máximo de uma coluna ou grupo de dados. Sua sintaxe com e sem GROUP BY é:

```sql
SELECT MAX(column_name) FROM table_name;
SELECT column_name, MAX(column_name) FROM table_name GROUP BY column_name;Ou ainda, com GROUP BY:
```

## MIN

A métrica MIN é utilizada para encontrar o valor mínimo de uma coluna ou grupo de dados. Sua sintaxe com e sem GROUP BY é:

```sql
SELECT MIN(column_name) FROM table_name;
SELECT column_name, MIN(column_name) FROM table_name GROUP BY column_name;
```

As métricas de agregação podem ser utilizadas em conjunto com outras cláusulas SQL, como WHERE e HAVING, para fornecer resultados mais específicos. A cláusula WHERE é usada para filtrar dados de acordo com uma condição específica. Por exemplo, para contar o número de linhas em uma tabela que atendem a uma determinada condição, você pode usar a métrica COUNT em conjunto com a cláusula WHERE. Exemplo:

```sql
SELECT COUNT(column_name) FROM table_name WHERE condition;
```

A cláusula HAVING é usada para filtrar grupos de dados de acordo com uma condição específica. Por exemplo, para contar o número de linhas em uma tabela agrupada que atendem a uma determinada condição, você pode usar a métrica COUNT em conjunto com a cláusula GROUP BY e a cláusula HAVING. Exemplo:

```sql
SELECT column_name, COUNT(column_name) FROM table_name GROUP BY column_name HAVING condition;
```

A condição na cláusula WHERE ou HAVING pode ser baseada em qualquer coluna da tabela ou em uma métrica de agregação.

**tldr;** HAVING é a mesma coisa que WHERE só que para agregações.
