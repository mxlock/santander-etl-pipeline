# 📊 Pipeline ETL com IA Generativa (Gemini 2.5 Flash)

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google%20Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)

Este projeto automatiza a criação de mensagens personalizadas de marketing para clientes bancários, utilizando inteligência artificial para gerar mensagens baseadas no ID do usuário.

## 🚀 Passo a Passo do Projeto

O pipeline segue o padrão **ETL** (Extract, Transform, Load):

1.  **Extract (Extração):** O projeto lê uma lista de IDs de clientes a partir de um arquivo `desafio.csv`.
2.  **Transform (Transformação):** Para cada ID, o modelo **Gemini 2.5 Flash** da Google é consultado via API para gerar uma frase de impacto curta (máximo 50 caracteres).
3.  **Load (Carga):** As mensagens geradas são consolidadas em um DataFrame do Pandas e exportadas para um novo arquivo `resultado_marketing.csv`.

## 🛠️ Tecnologias Utilizadas

* **Python 3**: Linguagem base.
* **Pandas**: Manipulação e análise de dados.
* **Google GenAI SDK**: Integração com o modelo Gemini 2.5 Flash.
* **VS Code**: Ambiente de desenvolvimento (Notebook interativo).

## 📋 Pré-requisitos

Antes de rodar o projeto, você precisará:

1.  Uma **API KEY** do Google AI Studio. [Obtenha aqui](https://aistudio.google.com/).
2.  Configurar a chave nas suas variáveis de ambiente com o nome `dio-api-dados`.
3.  Instalar as dependências:
    ```bash
    pip install -U google-genai pandas
    ```

## 📂 Estrutura de Arquivos

* `projeto.ipynb`: Notebook com o código principal.
* `desafio.csv`: Arquivo de entrada com os IDs dos clientes.
* `resultado_marketing.csv`: Arquivo gerado após o processamento da IA.

## ✒️ Autor

* **Thiago Ferreira** - (https://www.linkedin.com/in/thiago-ferreira-7a7376121/)
