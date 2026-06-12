# Passo a Passo de Execução

## Setup do Ollama

```bash
# 1. Instalar Ollama (ollama.com)
# 2. Baixar um modelo leve:
ollama pull gpt-oss

# 3. Testar se funciona:
ollama run gpt-oss "Olá!" 
```

# Código da Aplicação

Todo código-fonte está no arquivo `app-py`.

## Como Rodar

```bash
# 1. Instalar dependências:
pip install -r requirements.txt

# 2. Garantir que Ollama está rodando
ollama serve

# Rodar a app
streamlit run app.py 
```

## Estrutura Sugerida

```
src/
├── app.py              # Aplicação principal (Streamlit/Gradio)
├── agente.py           # Lógica do agente
├── config.py           # Configurações (API keys, etc.)
└── requirements.txt    # Dependências
```

## Exemplo de requirements.txt

```
streamlit
openai
python-dotenv
```

## Como Rodar

```bash
# Instalar dependências
pip install -r requirements.txt

# Rodar a aplicação
streamlit run .\src\app.py
```
