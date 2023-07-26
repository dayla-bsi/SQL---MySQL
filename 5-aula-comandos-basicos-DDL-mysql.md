DDL - Data Definition Language (LINGUAGEM DE DEFINIÇÃO DE DADOS)

1) CREATE
2) ALTER
3) DROP
4) TRUNCATE

CREATE
-
Criar um novo banco de dados: Após estabelecer a conexão, você pode criar um novo banco de dados usando o comando CREATE DATABASE. Por exemplo, para criar um banco de dados chamado "meu_banco_de_dados", você pode executar o seguinte comando:

```
CREATE DATABASE meu_banco_de_dados;
```

Selecionar um banco de dados: Para começar a trabalhar com um banco de dados específico, você precisa selecioná-lo usando o comando USE. Por exemplo, para selecionar o banco de dados "meu_banco_de_dados", use o seguinte comando:
```
USE meu_banco_de_dados;
```
Criar uma nova tabela: após criar o banco de dados, você pode criar uma nova tabela usando o comando:
```
CREATE TABLE minha_tabela(
id INT AUTO_INCREMENT PRIMARY KEY,
nome VARCHAR(50),
dtNasc DATE,
email VARCHAR(60)
);
```
Mais uma tabela, utilizando mais as constraints.
```
CREATE TABLE IF NOT EXISTS pessoa(
id INT AUTO_INCREMENT PRIMARY KEY,
nome VARCHAR(50) NOT NULL,
email VARCHAR(60) NOT NULL,
dtNasc DATE NOT NULL,
genero ENUM('M', 'F'),
peso DECIMAL (5,2),
altura DECIMAL (3,1),
nacionalidade VARCHAR(20) DEFAULT 'Brasil'
);
```

ALTER
-
ALTER em uma tabela para adicionar uma nova coluna:
```
ALTER TABLE pessoa ADD COLUMN profissao VARCHAR(30);
```
ALTER em uma tabela para excluir uma nova coluna:
```
ALTER TABLE pessoa DROP COLUMN profissao;
```
ALTER em uma tabela para adicionar uma nova coluna em um local específico na tabela, no exemplo a seguir, colocaremos na tabela a coluna "profissao" depois da coluna "genero" na tabela:
```
ALTER TABLE pessoa ADD COLUMN profissao VARCHAR(30) AFTER genero;
```
Se AFTER é depois então BEFORE é antes, correto? NÃO! Para adicionar na primeira coluna utilizamos o FIRST, logo, qualquer coluna depois da primeira pode ser trabalhada com AFTER. Exemplo  de uma coluna sendo adicionada como primeira coluna:
```
ALTER TABLE pessoa ADD COLUMN cod int FIRST;
```
ALTER em uma tabela para modificar os tipos primitivos e constraints das colunas. Por exemplo, na coluna "profissão" quando inserido os dados referentes a "profissão" o número de caracteres ultrapassa o tamanho definido no tipo VARCHAR(20), então modificamos os tipos primitivos e constraints usando MODIFY :
```
ALTER TABLE pessoa MODIFY COLUMN profissao VARCHAR(50);
```

DROP
-
Excluir um banco de dados: o comando DROP DATABASE exclui permanentemente um banco de dados:
```
DROP DATABASE meu_banco_de_dados;
```
Excluir uma tabela: o comando DROP TABLE exclui permanentemente uma tabela:
```
DROP TABLE minha_tabela;
```
