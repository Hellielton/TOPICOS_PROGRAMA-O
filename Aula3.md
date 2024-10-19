Aula 3 
O que é Engenharia de Prompt
A Engenharia de Prompts é uma disciplina emergente que se dedica a criar e otimizar instruções textuais, ou "prompts", que direcionam o comportamento dos LLMs para produzir respostas precisas e úteis. 
Este campo é essencial para maximizar a eficiência e a precisão dos modelos de linguagem, pois determina como esses modelos interpretam e respondem às solicitações dos usuários.

Formulação de entradas que orientam o comportamento dos modelos de linguagem.

A criação de prompts eficazes é um processo interativo que inclui planejamento, testes e refinamentos contínuos.

A EP deve prezar pela clareza, neutralidade e imparcialidade.

Escolha cuidadosa das palavras para evitar interpretações tendenciosas
EP inclui a criação e reestruturação de prompts existentes

Personalização de prompts para diferentes públicos e aplicações


Configurações da LLM
Temperatura - quanto menor a temperatura, mais determinísticos são os resultados
Tokens - cerca de 4 caracteres (english)
TopP - Se você está procurando respostas exatas e factuais, mantenha isso baixo

Prompts Básicos
O céu é
Melhorando o contexto:

Complete a sentença:
O céu é

- Estrutura

Estrutura Geral: O XML organiza as interações do agente da clínica como uma receita de bolo, dividida em seções específicas que detalham seu comportamento ao lidar com pacientes.
Elemento <Agent>: É o elemento principal que engloba toda a configuração do agente, como uma receita que descreve o objetivo.
Elemento <Description>: Explica o propósito geral do agente, como realizar agendamentos, consultas de exames e tirar dúvidas.
Elemento <Language>: Define o idioma e o tom da comunicação, neste caso, português informal e humanizado.
Elemento <CommunicationStyle>: Estabelece que o estilo de comunicação é informal, com dicas para o agente usar exemplos sem mencionar processos internos.
Elemento <FieldsConfigurator>: Configura ferramentas que validam dados antes de o agente responder, como instruções detalhadas na receita.
Elemento <Validations>: Define as regras para validação de informações, incluindo o uso do histórico completo de mensagens.
Elemento <Rules>: Regras que garantem que o agente siga diretrizes claras, como evitar fornecer informações erradas.
Elemento <Functions>: Define funções específicas do agente, como agendamento e consulta de exames.
Função Agendamento: Define regras sobre como o agente deve lidar com dados concretos e ser transparente quando não souber algo. O agente coleta e valida informações como nome, e-mail, médico, data e hora.
Função Consulta de Exames: Permite consultar resultados de exames.
Função Tira Dúvidas: Responde a perguntas dos pacientes com base nas informações do sistema.