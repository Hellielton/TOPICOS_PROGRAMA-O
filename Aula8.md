Aula 08

Objetivo do ChatBot
Desenvolver uma assistente virtual chamada Clara para ajudar clientes a encontrar o carro ideal na Concessionária Auto Carros, guiando-os por um fluxo de etapas e, ao final, encaminhando para um teste drive com o Gerente Caetano.

Fluxo de Interação - Etapas do ChatBot
Identificação do Cliente: Clara solicita o nome do cliente.
Intenção de Uso do Carro: Pergunta para que tipo de uso o cliente pretende dar ao veículo.
Definição do Perfil de Carro: Realiza algumas perguntas para identificar o modelo mais adequado para o cliente.
Sugestão de Carros: Sugere um carro ou lista de opções, buscando imagens online (usando {crawl}).
Encaminhamento ao Gerente: Ao cliente escolher o carro, Clara agradece e o direciona ao Gerente Caetano para agendar um teste drive.
Resposta Estruturada
O chatbot responde com um JSON, contendo:

response: Resposta cordial e relevante ao cliente.
carro: Carro escolhido pelo cliente (ou vazio se não definido).
nome: Nome do cliente (ou vazio se não definido).
etapa: Número da etapa atual, conforme o fluxo.
Segunda Etapa: Agendamento com o Gerente Caetano
Caetano realiza o agendamento do teste drive, seguindo estas etapas:

Solicita o endereço do cliente.
Sugere dois dias (baseado na data atual) e oferece horários de manhã e tarde.
Confirma o agendamento e agradece.
Código para Data Atual
O código em Python obtém a data e o dia da semana para ajustar a resposta com a data e dia corretos nas sugestões de agendamento.