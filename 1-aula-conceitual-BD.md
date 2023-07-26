BANCO DE DADOS
--  
Banco de dados é uma coleção organizada de informações - ou dados - estruturadas, normalmente armazenadas eletronicamente em um sistema de computador.

Existem diferentes tipos de bancos de dados, incluindo:
1) Bancos de dados relacionais: Utilizam o modelo relacional e armazenam dados em tabelas com esquemas predefinidos. São baseados na linguagem SQL (Structured Query Language).
2) Bancos de dados NoSQL: Utilizam modelos não relacionais e são mais flexíveis em termos de esquema e estrutura de dados.
3) Bancos de dados de grafos: São otimizados para armazenar e consultar dados baseados em relações complexas de grafos.
4) Bancos de dados em memória: Armazenam os dados na memória principal do computador para acesso mais rápido e desempenho otimizado.

A escolha do tipo de banco de dados depende das necessidades específicas do sistema e das características dos dados a serem armazenados. Em geral, os bancos de dados são essenciais para o gerenciamento eficiente de informações e para facilitar a tomada de decisões informadas.

NA DISCIPLINA UTILIZAREMOS O BANCO DE DADOS RELACIONAL!!!nBanco de Dados Relacional é um grupo de tabelas interligadas por RELACIONAMENTOS.

Sistema Gerenciador de Banco de DADOS (SGBD)
-
Sistema Gerenciador de Banco de Dados (SGBD) é um software projetado para facilitar o armazenamento, organização, recuperação, gerenciamento e manipulação de dados em um banco de dados. Ele atua como uma interface entre os usuários e o banco de dados, permitindo que os dados sejam armazenados de forma estruturada e eficiente.

Cada SGBD possui características distintas e é mais adequado para diferentes cenários e requisitos. A escolha do SGBD depende das necessidades específicas do projeto ou aplicação em questão. Alguns exemplos de SGBDs disponíveis
1)  MySQL: Um SGBD de código aberto muito popular, conhecido por sua velocidade e confiabilidade. É amplamente utilizado em aplicações web e de pequeno a médio porte.
2) MariaDB: É um fork do MySQL de código aberto, desenvolvida pelos criadores originais do MySQL. É uma opção popular para aqueles que desejam uma alternativa ao MySQL.
3) PostgreSQL: Outro SGBD de código aberto, que é altamente escalável e possui suporte para recursos avançados, como tipos de dados personalizados, funções e procedimentos armazenados.
4) Oracle Database: Um SGBD comercial líder de mercado, conhecido por sua robustez, escalabilidade e suporte a recursos avançados. É frequentemente utilizado em grandes sistemas corporativos.
5) Microsoft SQL Server: SGBD desenvolvido pela Microsoft, que possui uma forte integração com o ambiente Windows e oferece suporte a uma variedade de recursos para aplicações empresariais.
6) MongoDB: Um SGBD NoSQL orientado a documentos, projetado para armazenar dados no formato JSON-like (BSON). É amplamente utilizado em aplicações web e móveis que requerem escalabilidade horizontal.
7) Redis: Outro SGBD NoSQL, conhecido como um armazenamento de estrutura de dados em memória. É frequentemente usado para cache e gerenciamento de sessões em tempo real.
8) SQLite: Um SGBD incorporado, que é uma biblioteca C leve e rápida que não requer um servidor separado. É amplamente utilizado em aplicativos móveis e embarcados.
9) IBM Db2: Um SGBD corporativo desenvolvido pela IBM, que oferece suporte a várias plataformas e é conhecido por sua segurança e desempenho.
10) Amazon DynamoDB: Um serviço de banco de dados NoSQL totalmente gerenciado oferecido pela Amazon Web Services (AWS). É altamente escalável e é frequentemente usado para aplicações na nuvem.

MySQL/MariaDB
-
O MySQL/MariaDB é um SGBD amplamente utilizado, que oferece uma variedade de comandos para criar, manipular e consultar bancos de dados. Neste texto, vamos explorar alguns comandos iniciais no MySQL/MariaDB que são úteis para começar a trabalhar com esse SGBDR.

Para iniciar, é necessário estabelecer uma conexão com o servidor MySQL ou MariaDB. Isso pode ser feito por meio do comando mysql no terminal ou prompt de comando, seguido por informações como o nome de usuário, senha e host do servidor.
