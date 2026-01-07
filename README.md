# Desafio-santander-dev-week-2023-
Este projeto é uma solução ETL (Extract, Transform, Load) desenvolvida para o desafio Santander Dev Week 2023.

📋 Visão Geral do Projeto

Este projeto é uma solução ETL (Extract, Transform, Load) desenvolvida para o desafio Santander Dev Week 2023. O objetivo principal é criar mensagens de marketing personalizadas para clientes do banco Santander usando IA Generativa.
🔄 Fluxo do Processo ETL
1. EXTRACT (Extração)

    Entrada: Arquivo CSV (SDW2023.csv) contendo IDs de usuários

    Fonte de dados: API REST que fornece informações detalhadas dos clientes

    Endpoint: GET /users/{id} para buscar dados de cada cliente

2. TRANSFORM (Transformação)

    Processa os dados extraídos dos clientes

    Usa a API do ChatGPT (OpenAI) para gerar mensagens personalizadas

    Foco em mensagens sobre importância dos investimentos

    Customização baseada no perfil de cada cliente

3. LOAD (Carga)

    Envia as mensagens geradas de volta para a API

    Endpoint: PUT /users/{id} para atualizar a lista de "news" de cada usuário

    Atualiza o campo de notícias/marketing do cliente

   ⚠️ Problema Encontrado e Solução
Problema Original

A API oficial do desafio (https://sdw-2023-prd.up.railway.app) estava fora do ar, impedindo a conclusão do projeto.
Solução Implementada

 Eu peguei uma Fake API alternativa utilizando:

    FastAPI: Framework moderno e rápido para APIs em Python

    Python: Linguagem principal do projeto

    Docker: Para containerização e fácil execução
A API simula dados realistas de clientes bancários, incluindo:

    Informações pessoais

    Dados da conta bancária

    Informações do cartão

    Lista de notícias/mensagens

    🛠️ Tecnologias Utilizadas
Tecnologia	Finalidade
Python	Linguagem principal do ETL e da API
FastAPI	Framework para criação da API REST
Requests	Biblioteca para consumir APIs HTTP
OpenAI API	Geração de mensagens com IA
Pandas	Manipulação do arquivo CSV
Docker	Containerização da aplicação
Docker Compose	Orquestração de containers

    
