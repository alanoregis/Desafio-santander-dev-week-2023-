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
📋 Backend & API
Tecnologia	Versão	Finalidade	Documentação
Python	3.9+	Linguagem principal do projeto	https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white
FastAPI	0.100+	Framework para criação da API REST	https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white
Uvicorn	0.22+	ASGI server para execução da API	https://img.shields.io/badge/Uvicorn-499848?style=for-the-badge&logo=uvicorn&logoColor=white
📊 Processamento de Dados & ETL
Tecnologia	Versão	Finalidade	Documentação
Pandas	1.5+	Manipulação e análise de dados CSV	https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white
Requests	2.28+	Cliente HTTP para consumo de APIs	https://img.shields.io/badge/Requests-3776AB?style=for-the-badge&logo=python&logoColor=white
OpenAI API	-	Geração de mensagens com IA Generativa	https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white
🐳 Containerização & DevOps
Tecnologia	Versão	Finalidade	Documentação
Docker	20.10+	Containerização da aplicação	https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white
Docker Compose	2.17+	Orquestração de containers	https://img.shields.io/badge/Docker_Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white
📁 Formato de Dados & Serialização
Tecnologia	Finalidade	Badge
CSV	Armazenamento inicial dos IDs dos usuários	https://img.shields.io/badge/CSV-Data_Format-239120?style=for-the-badge
JSON	Formato de comunicação da API	https://img.shields.io/badge/JSON-Data_Format-000000?style=for-the-badge&logo=json&logoColor=white
🔧 Ferramentas de Desenvolvimento
Tecnologia	Finalidade	Badge
Git	Controle de versão	https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white
GitHub	Hospedagem do código	https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white
Virtual Env	Ambiente virtual Python	https://img.shields.io/badge/Virtual_Env-3776AB?style=for-the-badge&logo=python&logoColor=white


    
