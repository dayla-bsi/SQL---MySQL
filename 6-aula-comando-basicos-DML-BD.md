DML - Data Manipulation Language (LINGUAGEM DE MANIPULAÇÃO DE DADOS)
-
1) INSERT: insere dados em uma tabela.
2) SELECT: recupera/exibe dados/registros de uma tabela.
3) UPDATE: atualiza os dados existentes em uma tabela.
4) DELETE: deleta registros de uma tabela.

INSERT
-
   INSERT para inserir dados em uma tabela, utilizamos junto com o INSERTO o INTO, definindo entre parênteses todas as colunas existentes na tabela em questão e que receberão os dados utilizando a palavra VALUES, cada dado inserido a sua respectiva coluna, deve está dentro escrito dentro de aspas simples, o dado "DEFAULT" na última columa representa que a coluna já tem uma dado previamente definido na criação da tabela, isto é, 'Brasil':
   
   ```
   INSERT INTO pessoas
   (id, nome, email, dtNasc, genero, peso, altura, nacionalidade)
   VALUES
   ('1', 'Pedro', 'pedro@gmail.com', '2003-12-27', 'M', 'Engenheiro de Software','75.6', '1.80', DEFAULT);
```
O uso dos nomes dos campos/colunas entre parênteses é opcional colocá-los, o DEFAULT na coluna id, é referenciado o valor já inserido na tabela através do AUTO_INCREMENT utilizado na coluna id (PRIMARY KEY/CHAVE PRIMÁRIA) :


   ```
   INSERT INTO endereco VALUES
   (DEFAULT, 'Rua Pedro Peres', '574', 'Rio Branco', '93056-030', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua Afrânio Peixoto', '459', 'Duque de Caxias', '93090-010', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua Alberto Bins', '254', 'Arroio', '93080-010', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua Alagoas', '873', 'Arroio', '93120-140', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua Alexandre Nunes', '145', 'Arroio', '95039-450', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua Bento Gonçalves', '742', 'Centro', '93080-010', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua José de Alencar', '916', 'Rio Branco', '93076-030', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua Olavo Bilac', '118', 'Rio Branco', '93096-030', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua Acácias', '892', 'Feitoria', '93040-010', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua Walter Rost', '149', 'Feitoria', '93046-010', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua José Joaquim de Paula', '975', 'Feitoria', '93036-330', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua Walter Rost', '459', 'Feitoria', '93076-010', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Av. João Corrêa', '887', 'Rio Branco', '93096-030', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua nova 1', '149', 'Centro', '90000-000', 'São Leopoldo', 'RS', 'Brasil'),
   (DEFAULT, 'Rua nova 2', '975', 'Centro', '90000-000', 'São Leopoldo', 'RS', 'Brasil');
```

   

SELECT
-

Vejamos alguns dos muitos comandos SELECT. O SELECT *(asterisco) significa que todos os registros da tabela serão exibidos, depois do asterisco coplocamos a palavra FROM (de) que remete a tabela que irá ser trabalhada
 ```
SELECT * FROM pessoas;
```
Podemos também selecionar quais colunas queremos exibir, colocando os nomes das colunas desejadas seguidas de vírgula:
 ```
SELECT nome, email, genero FROM pessoas;
```
UPDATE
-
O UPDATE atualiza registros na tabela utilizando a palavra SET mdeiante alguma condição específica definida pela palavra WHERE.
```
UPDATE pessoas SET nome = 'João' WHERE id='1';
