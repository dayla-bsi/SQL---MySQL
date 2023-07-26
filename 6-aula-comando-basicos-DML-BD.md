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
