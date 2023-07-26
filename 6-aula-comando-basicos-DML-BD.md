DML - Data Manipulation Language (LINGUAGEM DE MANIPULAÇÃO DE DADOS)
-
1) INSERT: insere dados em uma tabela.
2) SELECT: recupera/exibe dados/registros de uma tabela.
3) UPDATE: atualiza os dados existentes em uma tabela.
4) DELETE: deleta registros de uma tabela.

   INSERT para inserir dados em uma tabela, utilizamos junto com o INSERTO o INTO, definindo entre parênteses todas as colunas existentes na tabela em questão e que receberão os dados utilizando a palavra VALUES, cada dado inserido a sua respectiva coluna, deve está dentro escrito dentro de aspas simples, o dado "DEFAULT" na última columa representa que a coluna já tem uma dado previamente definido na criação da tabela, isto é, 'Brasil':
   ```
   INSERT INTO pessoa
   (id, nome, dtNasc, genero, peso, altura, nacionalidade)
   VALUES
   ('1', 'Pedro', '2003-12-27', 'M', '75.6', '1.80', DEFAULT);
   
