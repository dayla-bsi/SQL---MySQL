Exercício do App Uber (Valendo 30 pontos)
--
Suponha que você está projetando um banco de dados para um serviço semelhante ao Uber, onde há motoristas, passageiros e viagens. 
Sua tarefa é criar um esquema de banco de dados com as seguintes tabelas:

Tabela "Motoristas":
Colunas: ID (Chave Primária), Nome, Placa do Veículo, Avaliação Média.

Tabela "Passageiros":
Colunas: ID (Chave Primária), Nome, Contato.

Tabela "Viagens":
Colunas: ID (Chave Primária), ID do Motorista (Chave Estrangeira), ID do Passageiro (Chave Estrangeira), Data e Hora, Origem, 
Destino, Distância, Preço.

Utilizando o CREATE E INSERT
--
*Tarefa 1*: 
Escreva o SQL para criar essas três tabelas em um banco de dados. Certifique-se de definir as chaves primárias e estrangeiras corretamente.

*Tarefa 2*: Insira alguns registros fictícios em cada tabela para simular motoristas, passageiros e viagens.
Tarefas

Utilizando o UPDATE
--
*Tarefa 1*: Atualize a placa do veículo de um motorista específico (por exemplo, Motorista1) para uma nova placa (por exemplo, "DEF789"):

*Tarefa 2*: Atualize em 0,5 a avaliação média de todos os motoristas que têm uma avaliação média atual maior ou igual a 4.0.

*Tarefa 2*: Atualize o preço de todas as viagens que ocorreram antes de uma determinada data (por exemplo, '2023-06-01') para um novo preço fixo (por exemplo, 20.0):

Utilizando o SELECT 
--

*Tarefa 1*: Escreva uma consulta SQL que retorne o nome do motorista, o nome do passageiro e a distância percorrida para todas as viagens com mais de 10 km.

*Tarefa 2*: Escreva uma consulta SQL que calcule a média das avaliações dos motoristas.

*Tarefa 3*: Escreva uma consulta SQL que liste os 10 melhores passageiros com base na quantidade total de dinheiro gasto em viagens.

*Tarefa 4*: Escreva uma consulta SQL que liste todos os motoristas que ainda não fizeram nenhuma viagem.

*Tarefa 5*: Escreva uma consulta SQL que retorne o número total de viagens feitas por cada motorista, classificando os resultados em ordem decrescente com base no número de viagens.

*Tarefa 6*: Escreva uma consulta SQL que retorne o passageiro que gastou mais em uma única viagem, incluindo o valor gasto e a data dessa viagem.

*Tarefa 7*: Escreva uma consulta SQL que liste as viagens feitas por um passageiro específico, incluindo o nome do motorista, data e hora da viagem e preço, ordenando as viagens pela data e hora.

*Tarefa 8*: Escreva uma consulta SQL que calcule a média de distância percorrida por todas as viagens e a média de preço das viagens.

Utilizando o DELETE 
--
*Tarefa 1*: Delete todas as viagens com uma distância menor que 5 km.

*Tarefa 2*: Delete todas as viagens realizadas antes de uma data específica (por exemplo, '2023-07-01').


Essas tarefas devem ajudá-lo a praticar a criação de um esquema de banco de dados e a escrever consultas SQL para extrair informações úteis de seus dados simulados relacionados ao Uber. 

