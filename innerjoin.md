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
