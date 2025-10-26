## Prompt Optimizer com Groq API

Projeto em Python para testar e avaliar prompts em modelos de linguagem usando a Groq API. Permite:

- Enviar diferentes tipos de prompts (zero_shot, few_shot, chain_of_thought).  
- Avaliar respostas automaticamente em clareza, relevância e precisão.  
- Visualizar métricas médias por tipo de prompt.  

🔧 **Tecnologias Utilizadas**  

- Python 3.x – Linguagem principal do projeto.  
- Pandas – Para manipulação e análise de dados.  
- Requests – Para chamadas HTTP à Groq API.  
- Matplotlib – Para visualização de métricas e gráficos.  
- Getpass – Para entrada segura da chave da API.  
- Groq API – Modelo de linguagem para processamento de prompts.  

⚡ **Requisitos**  

- Chave da Groq API válida.  

🚀 **Como usar**  

[![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/eduardaqueiroga/prompt-optimizer/blob/main/prompt-optimizer.ipynb)  

1. Abra o notebook no Colab clicando no botão acima.  
2. Execute a célula de configuração da API.  
3. Ao ser solicitado, digite sua chave Groq API (não ficará visível).  
4. O notebook executará os prompts de teste (zero_shot, few_shot, chain_of_thought) e coletará os resultados.  

📝 **Configuração de prompts**  

- `zero_shot` → max_tokens: 300  
- `few_shot` → max_tokens: 350  
- `chain_of_thought` → max_tokens: 600  

Você pode alterar `max_tokens` individualmente para cada prompt, garantindo respostas completas do modelo.  

📊 **Saída**  

- DataFrame com a resposta do modelo e avaliação automática  
- Gráficos de média de notas por tipo de prompt  

✅ **Observações**  

- O notebook foi testado com o modelo `llama-3.1-8b-instant` da Groq API  
- O uso de `getpass` garante que sua chave não fique visível  
- Se o modelo truncar a resposta, aumente `max_tokens` no prompt correspondente  

