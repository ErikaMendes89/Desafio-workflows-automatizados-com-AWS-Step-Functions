# 🚀 Workflows Automatizados com AWS Step Functions

Este repositório faz parte do desafio proposto no Bootcamp da DIO, com foco na criação e documentação de um fluxo automatizado usando **AWS Step Functions**.  
O objetivo é demonstrar na prática como orquestrar serviços serverless na AWS através de uma arquitetura escalável, observável e tolerante a falhas.

---

## 🧠 Objetivo do Desafio

Aplicar os conceitos aprendidos sobre Step Functions construindo um workflow real, integrando diferentes serviços da AWS e documentando o processo técnico de forma clara.

> **Meta principal:** consolidar seus workflows automatizados com AWS Step Functions

---

## 🏗️ Arquitetura Desenvolvida

O fluxo implementado segue uma arquitetura orientada a eventos e contém:

| Componente | Função no Workflow |
|------------|-------------------|
| **API Gateway** | Ponto de entrada da requisição |
| **Lambda (ingestão)** | Valida e envia o payload para a Step Function |
| **Step Functions** | Orquestra o fluxo principal |
| **Choice State** | Roteia o caminho com base em condições |
| **Parallel State** | Executa tarefas em paralelo (Lambda / DynamoDB / SQS) |
| **Map State** | Processa uma lista de itens de forma iterativa |
| **DynamoDB** | Armazena dados persistentes |
| **SQS** | Tarefas assíncronas e fila de fallback |
| **SNS** | Notificação final |
| **CloudWatch** | Logs, métricas e alarmes |
| **DLQ (Dead Letter Queue)** | Tratamento de erros com retry/catch |
| **IAM Roles** | Controle de permissão seguro e granular |

🖼️ **Diagrama do Workflow (PNG)**:  
*(adicione a imagem aqui no GitHub após upload)*

📄 **Arquivo `.drawio` editável** incluído no repositório

---

## 📌 Conceitos aplicados

- Orquestração vs Chaining de Lambdas
- Estados nativos (Choice, Map, Parallel, Retry, Catch)
- Boas práticas de resiliência e observabilidade
- Integração entre serviços serverless
- Arquitetura desacoplada orientada a eventos
- Dead Letter Queue & fallback seguro
- IAM mínimo necessário (principle of least privilege)

---
![Uploading кGIF.gif…]()


## 📂 Estrutura do Repositório

