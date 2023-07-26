Nessa aula, vamos aprender a usar o comando mais famoso da SQL: o SELECT.

Antes vamos criar (CREATE) e inserir (INSERT) dados em mais uma tabela para trabalharmos
```
CREATE TABLE IF NOT EXISTS cursos(
id INT AUTO_INCREMENT PRIMARY KEY,
nome VARCAHR(20) NOT NULL,
carga INT UNSIGNED,
ano INT UNSIGNED
);
```
```
INSERT INTO cursos VALUES
(DEFAULT, 'Ciência da Computação', '3840', '2017'),
(DEFAULT, 'Sistemas de Informação', '3830', '2018'),
(DEFAULT, 'Análise e Desenvolvimento de Sistemas', '1900', '2019'),
(DEFAULT, 'Engenharia da Computação', '3850', '2017'),
(DEFAULT, 'Engenharia de Software', '3820', '2020'),
(DEFAULT, 'Engenharia de Controle e Automação', '3810', '2017'),
(DEFAULT, 'Engenharia de telecomunicações', '3800', '2018'),
(DEFAULT, 'Sistemas para Internet', '1800', '2018'),
(DEFAULT, 'Ciência de Dados', '1100', '2021'),
(DEFAULT, 'Técnico em Informática para a Internet', '950', '2021'),
(DEFAULT, 'Técnico em Informática', '800', '2015'),
(DEFAULT, 'Medicina', '4500', '2015'),
(DEFAULT, 'Farmacia', '3500', '2016'),
(DEFAULT, 'Odontologia', '3400', '2016'),
(DEFAULT, 'Enfermagem', '3300', '2015'),
(DEFAULT, 'Nutrição', '3200', '2017');
```

SELECT
-
O SELECT * com asteriscos seleciona TODOS os registros/linhas e colunas FROM (da) tabela e os exibe.
```
SELECT * FROM cursos; 
```
O comando SELECT * from cursos, irá ordenar a tabela por ordem crescente do ID, mas para ordenar por qualquer outra coluna, colocvamos o ORDER BY e o nome da coluna:
```
SELECT * FROM cursos
ORDER BY nome; 
```
```
SELECT * FROM cursos
ORDER BY ano; 
```
Se quiser ordenar em ordem decrescente utiliza-se a palavra DESC:
```
SELECT * FROM cursos
ORDER BY nome DESC; 
```
```
SELECT * FROM cursos
ORDER BY ano DESC; 
```
OBSERVAÇÃO: O DESC utilizado como parâmetro NO SELECT "descendent". Porém, o DESC utilizado como comando SQL significa "describe", ou seja, descreve uma tabela, como no exemplo a seguir:
```
DESCRIBE cursos;
```
OU
```
DESC cursos;
```
Até agora utilizamos o SELECT * FROM, ou seja, exibindo todas as colunas. A seguir trabalharemos o SELECT com filtros. Isto porque nem todas as vezes que queremos fazer umas busca precisamos da base de dados inteira, então você pode filtrar para mostrar somente aquelas colunas que você precisa. No exemplo, não quero selecionar todas as colunas da tabela "cursos" mas somente as colunas nome e ano, e, ainda assim, também continuar ordenando-as. Tira o * e coloca as colunas que você quer que apareça.

```
SELECT nome, ano FROM cursos
ORDER BY nome;
```
Podemos também mudar as ordens das colunas, se quiser também ordenar por ano e depois também ordenar por nome:
```
SELECT ano, nome FROM cursos
ORDER BY ano, nome;
```

Se quisermos filtrar as linhas, ou seja, exibir somente tais registros, utilizamos a claúsula WHERE. POr exemplo, selecione todos os campos (SELECT * FROM) da tabela cursos onde o ano seja igual a 2017:
```
SELECT * FROM cursos
WHERE ano='2017'
ORDER BY nome; 
```
