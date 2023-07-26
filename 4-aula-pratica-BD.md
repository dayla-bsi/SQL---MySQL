SQL
-
Structured Query Language, "linguagem de consulta estruturada", é uma linguagem de domínio específico desenvolvida para gerenciar dados relacionais em um sistema de gerenciamento de banco de dados, ou
para processamento de fluxo de dados em um sistema de gerenciamento de fluxo de dados.

Conceitos CRUD 
-
CRUD é um acrônimo para as quatro operações básicas de um Banco de Dados. Tido por:

CREATE (CRIAR)

READ (SELECT)

UPDATE (ATUALIZAR)

DELETE (APAGAR)

DEFINIÇÃO DE LINGUAGEM
-
A linguagem SQL é dividida em quatro tipos de instruções de linguagem primárias:

DDL - Data Manipulation Language

DML - Data Definition Language

DCL - Data Definition Language

TCL - Transaction Control Language


DDL - Data Definition Language
---
São usadas para definir a estrutura de Banco de Dados ou esquema. Alguns exemplos:

1) CREATE: para criar objetos no banco de dados, o próprio banco de dados, tabelas, indexes, procedures, views, functions e triggers.
2) ALTER: altera a estrutura da base de dados, o próprio banco de dados, tabelas e indexes.
3) DROP: apaga objeto no banco de dados, o próprio banco de dados, tabelas, indexes, procedures, views, functions e triggers.
4) TRUNCATE: remover todos os registros de uma tabela, inclusive, todos os espaços alocados para uma tabela serão removidos.

DML - Data Manipulation Language
---
Os comandos DML são utilizados para o gerenciamento de dados dentro de objetos do banco. Alguns exemplos:

1) SELECT: recuperar dados do banco de dados.
2) INSERT: inserir dados em uma tabela.
3) UPDATE: atualiza os dados existentes em uma tabela.
4) DELETE: exclui registros de uma tabela.

DCL - Data Control Language
---
São usadas para definir acesso/controle dos dados/objetos.

1) GRANT: atribui os privilégios de acesso do usuário a objetos do banco de dados.
2) REVOKE: remove os privilégios de acesso aos objetos obtidos com o comando GRANT.

TCL - Transaction Control Language
---
São usados para gerenciar as mudanças feitas por instruções DML. Ele permite que as declarações a serem agrupadas em transções lógicas.

1) BEGIN TRANSACTION: inicia uma transação.
2) COMMIT: salvar o trabalho feito.
3) SAVE TRANSACTION: identificar um ponto em uma transação para que mais tarde você possa efetuar um ROLLBACK.
4) ROLLBACK: restaurar o banco de dados ao original desde o último COMMIT.

