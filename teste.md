
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

```
INSERT INTO alunos VALUES
(DEFAULT, 'Lucas', '455', '1999-07-25', '***.***.111-01'),
(DEFAULT, 'Lucas', '456', '2000-02-25', '***.***.222-02'),
(DEFAULT, 'Lucas', '457', '1996-09-25', '***.***.333-03'),
(DEFAULT, 'Lucas', '458', '2005-08-25', '***.***.444-04');
```

