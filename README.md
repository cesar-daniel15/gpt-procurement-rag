# GPT Procurement Intelligent - Arquitetura RAG

Este repositório contém os ficheiros de configuração em formato YML para a implementação da infraestrutura da Inteligência Artificial voltada para a análise de documentos. 

Estão disponíveis os seguintes modelos RAG: Open WebUI, PrivateGPT e LocalGPT

## Estrutura

| Container | Portas (Host:Container) |
| :--- | :--- |
| **ollama** | `11434:11434` |
| **rag-private** | `8002:8080` |
| **rag-webui** | `3001:8080` |

