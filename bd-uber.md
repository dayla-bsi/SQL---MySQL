Exercício do App Uber
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

Tarefas
--

*Tarefa 1*: 
Escreva o SQL para criar essas três tabelas em um banco de dados. Certifique-se de definir as chaves primárias e estrangeiras corretamente.

*Tarefa 2*: Insira alguns registros fictícios em cada tabela para simular motoristas, passageiros e viagens.

*Tarefa 3*: Escreva uma consulta SQL que retorne o nome do motorista, o nome do passageiro e a distância percorrida para todas as viagens com mais de 10 km.

*Tarefa 4*: Escreva uma consulta SQL que calcule a média das avaliações dos motoristas.

*Tarefa 5*: Escreva uma consulta SQL que liste os 10 melhores passageiros com base na quantidade total de dinheiro gasto em viagens.
