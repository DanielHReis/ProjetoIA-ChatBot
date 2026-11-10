# ProjetoIA-ChatBot

Chatbot simples de console chamado **BotBot**, desenvolvido em Python com [LangChain](https://python.langchain.com/) e a API da [Groq](https://groq.com/). O projeto foi criado com fins de **aprendizado** e para compor meu **portfólio/currículo**, demonstrando integração com modelos de linguagem (LLMs) e construção de uma conversa interativa com memória.

## Sobre o projeto

O `Chatbot.ipynb` implementa um assistente virtual que:

- Utiliza o modelo `openai/gpt-oss-120b` via `ChatGroq`;
- Mantém o histórico da conversa (memória de mensagens) ao longo da sessão;
- Responde de forma amigável, identificando-se como "BotBot";
- Encerra a conversa quando o usuário digita `x`.

Também há exemplos iniciais no notebook de uso de `ChatPromptTemplate` para tradução de expressões, incluindo variação com prompt de sistema.

## Tecnologias

- Python 3
- Jupyter Notebook
- LangChain (`langchain`, `langchain-core`)
- LangChain Groq (`langchain-groq`)
- Groq API

## Como executar

1. Instale as dependências:

   ```bash
   pip install langchain langchain-groq
   ```

2. Configure sua chave da Groq (recomenda-se usar variável de ambiente):

   ```bash
   # Windows (PowerShell)
   $env:GROQ_API_KEY = "sua_chave_aqui"
   ```

3. Abra o notebook `Chatbot.ipynb` em um ambiente Jupyter (ou VS Code) e execute as células.

4. Converse com o BotBot. Digite `x` para sair.

## Configuração da chave da API

Como obter a API Key da Groq
1. Acesse o GroqCloud Console.
2. Faça login ou crie uma conta gratuita.
3. Acesse a página API Keys.
4. Clique em Create API Key.
5. Defina um nome para sua chave, por exemplo, BotBot.
6. Clique em Submit para gerar sua chave.
7. Copie e guarde a API Key em um local seguro.
Atenção: a API Key é pessoal e não deve ser compartilhada ou publicada no GitHub.

## Autor

Daniel Henrique Reis e Silva — projeto de estudo para portfólio/currículo.
