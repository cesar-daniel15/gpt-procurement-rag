# GPT Procurement Intelligent - Arquitetura RAG

Este repositório contém os ficheiros de configuração em formato YML para a implementação da infraestrutura da Inteligência Artificial voltada para a análise de documentos. 

Estão disponíveis os seguintes modelos RAG: Open WebUI, PrivateGPT e LocalGPT

## Estrutura

| Container | Portas (Host:Container) |
| :--- | :--- |
| **[ollama](http://localhost:11434)** | `11434:11434` |
| **[rag-private](http://localhost:8002)** | `8002:8080` |
| **[rag-webui](http://localhost:3001)** | `3001:8080` |
| **[localgpt-frontend](http://localhost:3000)** | `3000:3000` |
| **[localgpt-backend](http://localhost:8000)** | `8000:8000` |
| **[localgpt-rag-api](http://localhost:8001)** | `8001:8001` |
