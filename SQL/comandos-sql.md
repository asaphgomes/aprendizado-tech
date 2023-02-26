## Lista de comandos gerais da linguagem SQL

| Comando    | Descrição                                                                                     |
| :--------- | :-------------------------------------------------------------------------------------------- |
| CREATE | Cria um novo objeto no banco de dados, como uma tabela, view, procedimento armazenado, função ou índice.<br>	- Sintaxe: ```CREATE DATABASE nome_do_banco_de_dados```;|
| DROP   | Remove uma tabela, view, índice, trigger ou outro objeto do banco de dados. <br> - Sintaxe: `DROP nome_do_objeto`; |
| BACKUP | Cria um backup completo ou parcial de um banco de dados do SQL Server.<br> - Sintaxe: ```BACKUP DATABASE nome_do_banco_de_dados TO DISK = 'path do arquivo'```;|
| TRUNCATE TABLE | Remove todos os registros de uma tabela, mantendo a estrutura da tabela. É mais rápido e consome menos recursos do que o comando DELETE.<br> - Sintaxe: `TRUNCATE TABLE nome_da_tabela`;|
| ALTER TABLE | Modifica a estrutura de uma tabela existente adicionando, removendo ou alterando colunas e restrições. <br> - Sintaxe: `ALTER TABLE nome_da_tabela ação`;|

🚧 Todos os comandos acima são genéricos, porém podem atuar de forma diferente se acionados corretamente. As subpáginas dos comandos estão em desenvolvimento.
