
```
CREATE DATABASE escola;

```
```
CREATE DATABASE alunos(
id INT AUTO_INCREMENT PRIMARY KEY,
nome VARCHAR(100) NOT NULL,
matricula VARCHAR(15) NOT NULL,
dtNasc DATE NOT NULL,
cpf VARCHAR(14) NOT NULL
);
```
TESTE

```
INSERT INTO alunos VALUES
(DEFAULT, 'Luiz Henrique', '455', '1999-07-25', '***.***.111-01'),
(DEFAULT, 'Rodrigo Fonseca', '456', '2000-02-25', '***.***.222-02'),
(DEFAULT, 'Gustavo José', '457', '1996-09-25', '***.***.333-03'),
(DEFAULT, 'Matheus Henrique', '458', '2005-08-25', '***.***.444-04');
```
teste
```
UPDATE alunos SET nome='Luiz Henrique Silva'
WHERE id='1';
```

TESTED

```
DELETE FROM alunos WHERE matricula='458';
```

```
SELECT * FROM alunos;
```
```
SELECT nome, matricula FROM alunos;
```

