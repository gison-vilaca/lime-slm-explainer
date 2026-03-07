# Adaptive LIME Explainer with Local SLMs

Este projeto avalia como escolher de maneira adaptativa o número de perturbações do LIME para obter uma explicabilidade de texto coerente para uma *query* $x$, utilizando Pequenos Modelos de Linguagem (SLMs) executados localmente.

A abordagem é inspirada na tradução de explicações matemáticas complexas para linguagem acessível a públicos não técnicos. 

## Tecnologias
* **LIME**: Para geração de interpretabilidade local.
* **Docker Model Runner**: Para execução local e otimizada de modelos como `qwen2.5` e `ibm-granite-4.0-nano` via uma API compatível com OpenAI.
* **Python & Jupyter**: Para análise e avaliação das perturbações.

## Como rodar
1. Certifique-se de que o **Docker Desktop** está rodando com o recurso *Model Runner* ativado.
2. Faça o pull e inicie o modelo desejado no terminal do host:
   `docker model pull qwen2.5`
   `docker model run qwen2.5`
3. Suba o ambiente de desenvolvimento:
   `docker compose up -d`
4. Acesse o Jupyter Notebook em `localhost:8888`.
