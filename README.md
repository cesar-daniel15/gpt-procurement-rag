# GPT Procurement Intelligent - Arquitetura RAG

Este repositório contém os ficheiros de configuração em formato YML necessários para implementar a infraestrutura de Inteligência Artificial destinada à análise de documentos.

A solução disponibiliza três ferramentas RAG:

* Open WebUI
* PrivateGPT
* LocalGPT

O objetivo é disponibilizar ferramentas de Inteligência Artificial de forma simples e acessível, permitindo a interação com documentos e a obtenção de respostas de forma autónoma.

## Estrutura

| Ferramenta     | URL                     |
| :------------- | :---------------------- |
| **Open WebUI** | `http://localhost:3001` |
| **PrivateGPT** | `http://localhost:8002` |
| **LocalGPT**   | `http://localhost:3000` |

O ambiente utiliza Docker para organizar e executar as diferentes ferramentas RAG.

## Requisitos

Antes de iniciar a instalação, é necessário ter:

* Docker Desktop
* Git

Em ambiente Windows, o Docker Desktop pode ser instalado através da Microsoft Store.

## Instalação

### 1. Clonar o projeto

No terminal, execute:

```bash
git clone https://github.com/cesar-daniel15/gpt-procurement-rag.git
```

Entre no diretório do projeto:

```bash
cd gpt-procurement-rag
```

### 2. Iniciar a estrutura Docker

Execute:

```bash
docker compose up
```

A estrutura utiliza imagens pré-compiladas. O processo de instalação pode demorar aproximadamente 5 a 10 minutos.

### 3. Instalar o LocalGPT

O LocalGPT é instalado separadamente através do Git Bash.

Clone o repositório:

```bash
git clone https://github.com/promtengineer/localgpt
```

Entre na pasta:

```bash
cd localGPT
```

De seguida, execute o ficheiro `.start-docker.sh` para construir e iniciar automaticamente os containers do LocalGPT, constituídos pelas componentes Frontend, Backend e API.

## Ordem de inicialização

Depois da instalação, o container do Ollama (`core-ollama`) deve ser iniciado primeiro.

De seguida, deve ser iniciada a ferramenta RAG pretendida:

* Open WebUI
* PrivateGPT
* LocalGPT

## Interfaces Gráficas

Após a inicialização, as ferramentas podem ser acedidas através dos seguintes endereços:

* **Open WebUI:** http://localhost:3001
* **PrivateGPT:** http://localhost:8002
* **LocalGPT:** http://localhost:3000

A estrutura permite disponibilizar ferramentas de Inteligência Artificial para a análise de documentos através de uma instalação simples e acessível.
