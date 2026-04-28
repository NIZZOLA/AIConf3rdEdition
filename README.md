# 🚀 Criando Múltiplos Agentes com Agent Framework + Azure AI Foundry

Este repositório contém os materiais da palestra apresentada no **AI Conference - 3 Edition 2026 (Brasil)**, com foco na criação de soluções modernas utilizando múltiplos agentes com o **Microsoft Agent Framework** integrado ao **Azure AI Foundry**.

## 📄 Materiais da Apresentação
📄 Slides :  

- 📕 [Slides em PDF (visualização)](https://github.com/NIZZOLA/AIConf3rdEdition/blob/main/docs/AI-Conf3Edition-agents-agent-framework.pdf)
- 📊 [Slides em PowerPoint (editável)](https://github.com/NIZZOLA/AIConf3rdEdition/blob/main/docs/AI-Conf3Edition-agents-agent-framework.pptx)
---

## 🎯 Objetivo

Apresentar como construir aplicações inteligentes baseadas em múltiplos agentes, explorando:

- Orquestração de agentes
- Workflows baseados em grafos
- Integração com Azure AI Foundry
- Uso de ferramentas (Tools) locais e remotas (MCP)

---

## 🧠 Conceitos Abordados

### 🔹 Azure AI Foundry

Plataforma da Microsoft para desenvolvimento de soluções com IA:

- Catálogo de modelos (OpenAI, customizados, etc.)
- Serviços como:
  - Azure AI Search
  - Machine Learning
  - Content Safety
- Observabilidade e governança integradas :contentReference[oaicite:2]{index=2}

---

### 🔹 Agentes vs Workflows

| Agentes 🧠 | Workflows ⚙️ |
|----------|-------------|
| Dinâmicos (baseados em LLM) | Determinísticos |
| Tomada de decisão autônoma | Fluxo controlado |
| Ideal para chat e exploração | Ideal para processos estruturados |

> 💡 Regra de ouro: Se dá para resolver com código determinístico simples, não use agente.

---

## 🧩 Arquitetura Multi-Agente

A palestra apresenta três padrões principais:

- **Sequencial** → saída de um agente alimenta o próximo  
- **Concorrente** → múltiplos agentes em paralelo  
- **Handoff** → transferência dinâmica entre agentes especializados :contentReference[oaicite:3]{index=3}  

---
### 🔹 Microsoft Agent Framework

O **Agent Framework** é a evolução do **Semantic Kernel** e **AutoGen**, trazendo uma abordagem *Agent-First*, projetada desde o início para aplicações modernas de IA.

Principais características:

- Modelo unificado para **.NET e Python**
- Foco em aplicações **enterprise**
- Gerenciamento avançado de estado e sessão
- Telemetria e observabilidade nativas :contentReference[oaicite:1]{index=1}

---

## 🛠️ Exemplo Prático (.NET)

```bash
dotnet add package Microsoft.Agents.AI.Foundry --prerelease