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
