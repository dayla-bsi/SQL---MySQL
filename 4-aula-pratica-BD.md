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

CONSTRAINTS
-
Constraint são utilizadas para especificar regras de armazenamentos de dados nas tabelas e garantir integridade.

TIPOS:

NOT NULL: Garante que uma coluna não recebera valor nulo.
UNIQUE: Garante que o valores em uma coluna sejam únicos. Exemplo: cpf.
PRIMARY KEY (Chave primária): Chave unica, linha exclusiva que representa cada registro/linha/tupla da tabela
FOREIGN KEY (Chave estrangeira): estabelece o relacionamento entre duas tabelas, transportando o id de uma tabela para a tabela que recebe o relacionamento.
DEFAULT: Define um valor padrão para uma coluna quando nenhum valor é especificado. Ex.  no campo pais posso definir no script para todos como 'Brasil', consequentemente, já fica inserido automaticamente na tabela.
INDEX: Usado para criar e recuperar dados do banco de dados com melhor performance.

PARA ATRIBUTOS NÚMERICOS:

UNSIGNED: impede que a coluna que tenha o tipo de dado inteiro armazene números negativos. Quando omitimos o atributo UNSIGNED em uma coluna de tipos de dados numéricos, seu padrão é SIGNED, permitirá valores negativos.
ZEROFILL: provoca efeitos de autopreenchimento de espaços não utilizados em uma coluna com zeros.
AUTO_INCREMENT: é bastante utilizado para gerar chave primária, isto é, gerando automaticamente um identificador único.
