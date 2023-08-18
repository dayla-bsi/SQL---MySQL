Criar (CREATE) as tabelas
```
CREATE TABLLE cliente(
id INT NOT NULL AUTO_INCREMENT,
nome VARCHAR (30) NOT NULL,
PRIMARY KEY(id)
);
```
```
CREATE TABLE compras(
id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
valor DECIMAL(6,2) NOT NULL,

id_cliente INT NOT NULL,
FOREIGN KEY(id_cliente) REFERENCES cliente (id)
);
```
Inserir (INSERT) dados nas tabelas
```
INSERT INTO cliente VALUES
(DEFAULT, 'Gustavo'),
(DEFAULT, 'Leonardo'),
(DEFAULT, 'Vitor'),
(DEFAULT, 'Aline'),
(DEFAULT, 'José');
```
```
INSERT INTO cliente VALUES
(DEFAULT, '1851.00', '1'), //Gustavo
(DEFAULT, '1950.00', '4'), //Aline
(DEFAULT, '1100.00', '3'), //Vitor
(DEFAULT, '1560.00', '2'); //Leonardo
```
Atualizar (UPDATE) dados da tabela
```
UPDATE cliente SET nome = 'Henrique' WHERE id='5';
```
Deletar (DELETE) dados da tabela. OBS.:Apagar registros específicos mediante uma condição. Se quisesse apagar todos de uma vez usava a claúsula TRUNCATE nomeDaTabela;
```
DELETE FROM cliente WHERE id='5';
```
INNER JOIN
-
**Junção (JOIN) interna de DUAS tabelas que se relacionam.**
```
SELECT * FROM cliente JOIN compras ON cliente.id=compras.id_cliente;
```
**Exercício aula passada (16/08)**

Suponha que temos duas tabelas: uma chamada "Clientes" com as colunas "ID" e "Nome", e outra chamada "Compras" com as colunas "ID_Cliente" e "Valor". O exercício é encontrar o nome dos clientes que fizeram compras com valores superiores à média de todos os valores de compra.

```
SELECT * FROM cliente JOIN compras ON cliente.id=compras.id_cliente
WHERE compras.valor (SELECT AVG (valor) FROM compras);
```
ou colocando no registro colunas específicas
```
SELECT cliente.nome FROM cliente JOIN compras ON cliente.id=compras.id_cliente
WHERE compras.valor > (SELECT AVG (valor) FROM compras);
```
ou criando um atributo para referenciar a tabela. Ex.: Podemos chamar a tabela cliente de c.
```
SELECT * FROM cliente c JOIN compras co ON c.id=co.id_cliente
WHERE co.valor > (SELECT AVG (valor) FROM compras);
```
**Junção (JOIN) interna de VÁRIAS tabelas que se relacionam.**

```
CREATE TABLE aluno(
id INT NOT NULL AUTO_INCREMENT,
nome VARCHAR (30) NOT NULL,
cpf VARCHAR (14) NOT NULL,
PRIMARY KEY(id)
);
```

```
CREATE TABLE curso(
id INT NOT NULL AUTO_INCREMENT,
nome VARCHAR (30) NOT NULL,
carga_hora INT NOT NULL,
PRIMARY KEY(id)
);
```
```
CREATE TABLE vinculo_aluno_curso(
id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
faltas INT NOT NULL,

id_aluno INT NOT NULL,
id_curso INT NOT NULL,

FOREIGN KEY (id_aluno) REFERENCES aluno(id),
FOREIGN KEY (id_curso) REFERENCES curso(id)
);
```
**INNER JOIN de VÁRIAS tabelas**
```
SELECT * FROM aluno JOIN vinculo_aluno_curso ON aluno.id=vinculo_aluno_curso.id_aluno JOIN curso ON curso.id=vinculo_aluno_curso.id_curso;
```
