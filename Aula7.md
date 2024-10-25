Resumo da aula 06 com a instalação do Docker

Docker é uma plataforma de containerização que permite empacotar uma aplicação com todas as suas dependências em um container, o que facilita a execução consistente em qualquer sistema com Docker.

Uso do WSL 2 + Docker no Desenvolvimento
Para desenvolvedores Windows, o uso do Docker com WSL 2 simplifica o processo de configurar e executar ambientes Unix-like, que geralmente é mais rápido e independente de compatibilidade.

Modos de Executar o Docker no Windows
Docker Desktop com WSL2:

Executa sobre a plataforma de máquinas virtuais (Hyper-V) e permite rodar containers Docker no ambiente Linux.
Vantagens: Interface visual, suporte a Kubernetes, menos consumo de recursos.
Desvantagens: Consumo inicial de memória (1GB+), necessidade de reiniciar o Docker ocasionalmente.
Docker Engine (Nativo) no WSL2:

Permite instalar o Docker diretamente no WSL2, reproduzindo a experiência de Docker no Linux.
Vantagens: Menor consumo de memória e maior eficiência.
Desvantagens: Necessidade de reconfigurar Docker para instâncias adicionais do WSL.
Instalação e Configuração
Configurar WSL:

Atualize para a última versão com wsl --update e defina o WSL2 como padrão com wsl --set-default-version 2.
Instale o Ubuntu ou outra distribuição Linux com wsl --install.
Instalar Docker no WSL2 (Ubuntu):

Configure o repositório do Docker e instale o Docker Engine usando o apt.
Containerização de uma Aplicação Node.js
Preparação do Projeto:

Clone um repositório Node.js de exemplo e teste a aplicação localmente.
Criar um Dockerfile:

Especifique a imagem base do Node.js, copie dependências e exponha a porta 3000.
Construir e Executar a Imagem:

Use docker build para criar a imagem e docker run para rodá-la, acessando a aplicação em http://localhost:3000.
Utilizando Docker Compose
O Docker Compose permite orquestrar múltiplos containers (como banco de dados e servidor) com um arquivo docker-compose.yml, útil para aplicações complexas que dependem de múltiplos serviços.

Exemplo de Docker Compose com Node.js e MySQL:

Define serviços como o app Node.js e um banco de dados MySQL, com variáveis de ambiente específicas para cada serviço.
Resumo Final
Docker com WSL2 é uma solução eficiente para desenvolvimento no Windows, integrando um ambiente Linux ao sistema e facilitando a containerização e orquestração com Docker Compose.