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

A chave da Groq não deve ser versionada. Existem duas formas de fornecê-la:

1. **Arquivo local `api_key.py`** (recomendado para este projeto):
   - Copie `api_key.example.py` para `api_key.py`;
   - Substitua `"sua_chave_aqui"` pela sua chave real;
   - `api_key.py` está no `.gitignore` e **não** será enviado ao GitHub.

2. **Variável de ambiente** `GROQ_API_KEY`:
   - Se `api_key.py` não existir, o notebook tenta ler de `os.getenv('GROQ_API_KEY')`.

O notebook contém uma chave de API hardcoded apenas para fins de estudo. Em projetos reais, utilize variáveis de ambiente e nunca versione segredos no repositório.

## Autor

Daniel Henrique Reis — projeto de estudo para portfólio/currículo.
