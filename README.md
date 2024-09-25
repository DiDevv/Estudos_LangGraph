# Visão Geral

O LangGraph é um framework para construção de softwares com LLMs que permite a criação de agentes mais confiáveis e gerenciáveis. A estrutura do framework é focada em grafos cíclicos (Diferente de frameworks com DAGs que utilizam grafos acíclicos tipo o LangChain). 
Os grafos cíclicos permitem que os agentes não sigam apenas uma ordem linear para tomada de decisão, o que facilita a criação de agentes mais "inteligentes" e confiáveis.
Por ter sido criado pelos mesmos criadores do LangChain, é possível realizar a integração com o LangSmith e o LangChain (integração essa que NÃO é obrigatória).

Como base inicial para estudos, estou utilizando a documentação do LangGraph e alguns outros cursos disponíveis na internet, a lista de todos eles se encontram abaixo: 

1. [LangGraph Documentation](https://langchain-ai.github.io/langgraph/tutorials/introduction/)

---
# Instalação

```Python
pip install -U langgraph
```

---

# Execução do código

Certifique-se de criar um arquivo .env contendo:

OPENAI_API_KEY = SUA API DA OPENAI ( Ou alguma chave de API de LLMs (Certifique-se de modificar o openai_api_key = os.getenv("OPENAI_API_KEY") para o nome que você definir, e modificar a chamada de modelo do LangChain.)

Se quiser monitorar todos as suas interações pelo LangSmith, certifique-se de adicionar:
LANGCHAIN_TRACING_V2=true
LANGCHAIN_ENDPOINT="https://api.smith.langchain.com"
LANGCHAIN_API_KEY="Sua api do langchain"
LANGCHAIN_PROJECT="Nome do seu projeto no langsmith"
