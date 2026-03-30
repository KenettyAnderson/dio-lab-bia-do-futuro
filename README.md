# 🤖 BIA: Assistente Financeira com GenAI e Pandas

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458.svg)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT_3.5_Turbo-green.svg)

## 📖 Sobre o Projeto
Este projeto é a entrega do Desafio Final do Bootcamp **Bradesco - GenAI & Dados** da DIO. 

O objetivo é aplicar conceitos de **IA Generativa no mercado financeiro**. Para ir além de um simples chatbot, desenvolvi um pipeline **ETL (Extract, Transform, Load)** autossuficiente que simula a análise automatizada de um extrato bancário. A assistente virtual (inspirada na BIA) lê um conjunto de dados, analisa o comportamento de consumo e devolve um relatório personalizado com dicas de educação financeira.

## 🚀 Diferenciais desta Implementação
Em vez de depender de arquivos `.csv` externos que podem causar erros de diretório (`FileNotFoundError`) durante a avaliação do código, optei por construir um **código 100% autossuficiente**. 
1. **Extract:** Os dados transacionais são gerados e estruturados diretamente na memória usando dicionários e a biblioteca `Pandas`.
2. **Transform:** Os dados tabulares são convertidos em texto de contexto e enviados à API da OpenAI. O modelo foi configurado com um *System Prompt* rigoroso para atuar como uma consultora empática e analítica.
3. **Load:** O sistema exibe o DataFrame original e carrega a resposta gerada pela IA, entregando valor imediato ao usuário.

## 💻 Como Executar
1. Clone este repositório ou abra o arquivo `.ipynb` no Google Colab.
2. Certifique-se de ter as bibliotecas instaladas (`pip install openai pandas`).
3. Insira a sua chave de API da OpenAI na variável `os.environ['OPENAI_API_KEY']`.
4. Execute o script. O programa irá gerar os dados, enviar para análise e imprimir o relatório financeiro.

## 📊 Exemplo de Saída
**Dados Analisados:** R$ 970,50 divididos entre Supermercado, Lazer e Delivery.

**Resposta da IA:**
> Olá! Analisei seu extrato e percebi que você teve um total de gastos de R$ 970.50 neste mês. Fique tranquilo, estamos aqui para organizar isso juntos! 🤝
> 
> O principal ponto de atenção no seu extrato são os gastos repetitivos com **Delivery**, que somaram R$ 260.50 em três pedidos diferentes. Embora seja prático, essas pequenas despesas frequentes acabam pesando bastante no orçamento final. 🍔🛵
> 
> **Dica da BIA:** Que tal estipular um limite mensal ou semanal para gastos com delivery? Você pode planejar as refeições da semana após a sua ida ao supermercado. Assim, você economiza dinheiro e ainda pode descobrir novos talentos na cozinha! 🍳💰
