# 🤖 BIA: Assistente Financeira com GenAI e Pandas

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458.svg)](https://pandas.pydata.org/)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT_3.5_Turbo-green.svg)](https://openai.com/)

> Agente de IA Generativa que atua como educadora financeira, analisando extratos bancários de forma empática e gerando insights práticos de economia utilizando um pipeline ETL 100% autossuficiente.

## 💡 O Que é a BIA Analisadora?

A BIA é uma assistente virtual focada em transformar dados numéricos frios (um extrato) em conselhos de organização financeira acolhedores e fáceis de entender.

**O que a BIA faz:**
* ✅ Analisa dados tabulares e identifica onde o cliente gasta mais.
* ✅ Gera resumos acolhedores usando linguagem empática e emojis.
* ✅ Fornece dicas práticas e educacionais de economia.

**O que a BIA NÃO faz (Foco em Segurança):**
* ❌ Não recomenda compra de ativos (ações, criptomoedas, etc).
* ❌ Não exige conexão com bancos reais ou upload de planilhas sensíveis.
* ❌ Não alucina taxas de juros ou produtos financeiros inexistentes.

## 🏗️ Arquitetura (Pipeline ETL)

```mermaid
flowchart TD
    A[Dados Mockados] -->|Extract| B(Pandas DataFrame)
    B -->|Transform Context| C[OpenAI API - GPT-3.5]
    C -->|System Prompt| D{Análise de Perfil}
    D -->|Load| E[Relatório Financeiro na Tela]
