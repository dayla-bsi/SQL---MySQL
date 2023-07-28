
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
(DEFAULT, 'Lucas', '455', '1999-07-25', '***.***.111-01'),
(DEFAULT, 'Pedro', '456', '2000-02-25', '***.***.222-02'),
(DEFAULT, 'João', '457', '1996-09-25', '***.***.333-03'),
(DEFAULT, 'Mateus', '458', '2005-08-25', '***.***.444-04');
```

