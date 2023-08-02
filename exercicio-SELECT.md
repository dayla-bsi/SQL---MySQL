Certamente, no nosso sistema de uma universidade denominado no Banco de Dados de "unisenac" tem uma tabela de Docentes, que já possui os seguintes atributos:

- **Tabela "Docentes":**
  - Atributos:
    - `id` (INT): chave primária que identifica exclusivamente cada Docente
    - `nome` (VARCHAR): nome do professor
    - `cpf` (VARCHAR): cpf do professor
    - `formacao` (VARCHAR): curso de formação do professor
    - `salario` (DECIMAL): salario do professor
    - `dataAdmissao` (DATE): : Data de admissão ou contratação do professor
    - `especializacao`  (VARCHAR): se o professor possuir aguma especialização, inserir qual.

   
**Exercício prático**  

1º **Alterar (ALTER)** o nome da tabela "docentes" para "professores" para ficar mais intuitivo.

2º **Alterar (ALTER)** a tabela "professores" adiconando três novas colunas:
   
    - "genero" - adiconar depois da coluna "cpf"
    - "carga_horaria" - adiconar depois da coluna "formacao"
    - "nível_academico" - adiconar depois da coluna "espec"
    
3º **Inserção (INSERT) de Dados e Manipulação**
Inserir os dados de professores na tabela.

4º **Consultas e relatórios (SELECT)**
Para realizar consultas no Banco de Dados e obter informações relevantes. Faça as seguintes onsultas na tabela "professores":

    1) Uma lista de todas as professoras (mulheres);
    2) Uma lista com os dados  de todos aqueles que foram admitidos entre 1/jan/2020 e 31/Dez/2021;
    3) Uma lista de todos os professores (homens) formados em Ciência da Computação;
    4) Uma lista de todas as mulheres com nível de mestrado  e que tem o nome iniciado com a letra "A";
    5) Uma lista com todos os nomes, cpf, carga de trabalho, nivel academico que ganham menos que 12.000;
    6) Uma lista com o maior salario entre os homens com nível de doutorado;
    7) Uma lista com o menor salario entre os mulheres com nível de doutorado;
    8) Uma lista com a média de salário de todos os professores;
    9) Uma lista com o menor salário entre todos os professores;
    10) Quantos professores (todos - homens e mulheres) ganham mais que 12.000;
    11) Quantas professoras ganham mais que 12.000;
