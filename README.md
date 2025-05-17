# 💪 GymBot: Seu Plano de Treino Inteligente 

## 🧐 Visão Geral

Este projeto consiste em um chatbot inteligente capaz de gerar planos de treinamento personalizados com base nas informações fornecidas pelo usuário. Utilizando o poder dos modelos de linguagem do Google (Gemini API) e princípios de treinamento físico. O chatbot interage com o usuário para entender seus objetivos, nível de atividade, restrições e preferências, e então cria um plano de exercícios semanal detalhado e alinhado com as recomendações da Organização Mundial da Saúde (OMS).

Por enquanto, é um projeto muito simples. Mas primeiro a gente começa e depois melhora ...😄. A ideia é que seja possível aprimorar em breve, incluindo as melhorias descritas no item de próximos passos, como vídeos demonstrativos de exercícios, integrar com o Google Calendar e muito mais.

## ✨ Funcionalidades Principais

* **Coleta de Dados do Usuário:** Através de uma série de perguntas interativas, o chatbot coleta informações essenciais para a criação do plano.
* **Geração da Estrutura Geral do Plano:** Um agente de IA (Agente 1) processa os dados do usuário e utiliza a Gemini API para gerar uma estrutura geral do plano de treinamento semanal, incluindo a divisão dos dias de treino e os grupos musculares a serem trabalhados.
* **Detalhamento do Plano de Exercícios:** Um segundo agente de IA (Agente 2) pega a estrutura geral e os dados do usuário para detalhar o plano, selecionando exercícios específicos, definindo séries, repetições, descanso, e incluindo sugestões de aquecimento e resfriamento.
* **Consideração das Diretrizes da OMS:** O Agente 2 leva em conta as recomendações da OMS sobre atividade física para a idade, nível de atividade e objetivos do usuário, buscando alinhar o plano gerado com essas diretrizes.
* **Classificação e Duração dos Exercícios:** Cada exercício no plano é classificado como aeróbico ou de fortalecimento, e uma duração estimada é fornecida.
* **Comparativo com a OMS:** Ao final do plano, o chatbot apresenta a recomendação da OMS para o usuário e compara o plano gerado com essas diretrizes.
* **Formatação em Markdown:** O plano de exercícios é apresentado em um formato Markdown claro e organizado, facilitando a leitura.

## ⚙️ Arquitetura

O projeto utiliza uma arquitetura com dois agentes de IA:

1.  **Agente 1 (agente\_planoGeralExerc):** Responsável por interagir com o usuário, coletar e organizar os dados, e utilizar a Gemini API para obter a estrutura geral do plano de treinamento.
2.  **Agente 2 (agente\_planoFinalExerc):** Responsável por detalhar o plano de exercícios com base na estrutura geral, nos dados do usuário e nas diretrizes da OMS. Este agente também classifica os exercícios, estima a duração e realiza o comparativo com as recomendações da OMS.

## 💻 Tecnologias Utilizadas

* **Python:** Linguagem de programação principal.
* **Google AI Python Library (genai):** Para interagir com a Gemini API.
* **Google-adk:** Para a criação e gerenciamento dos agentes de IA.
* **IPython.display (display, Markdown):** Para exibir o plano de exercícios formatado em Markdown (útil em ambientes como Google Colab e Jupyter Notebook).

## ▶️ Como Executar

1.  **Pré-requisitos:**
    * Conta Google com acesso à Gemini API.
    * Chave de API do Gemini configurada no ambiente.
    * Python 3.x instalado.
    * Bibliotecas listadas em "Tecnologias Utilizadas" instaladas (`pip install google-generativeai ipython [outras_bibliotecas]`).

2.  **Execução:**
    * Clone ou faça o download do código do projeto.
    * Execute o script Python principal (ex: `main.py`).
    * Siga as instruções do chatbot para fornecer suas informações.
    * O plano de treinamento personalizado será exibido na tela.

## 🚀 Próximos Passos e Melhorias Futuras

* Implementação da busca e inclusão de links para vídeos demonstrativos dos exercícios.
* Integração com o Google Calendar para agendar os treinos.
* Adição de suporte para diferentes níveis de personalização e objetivos mais específicos.
* Implementação de um sistema de feedback para o usuário avaliar o plano e fornecer informações para futuras melhorias.
* Persistência dos dados do usuário e dos planos gerados.
* Interface de usuário mais amigável (ex: utilizando um framework web como Flask ou Streamlit).

## ⚠️ Considerações Importantes

* **Consulta Médica:** Antes de iniciar qualquer programa de exercícios, é fundamental consultar um médico ou profissional de educação física para avaliar sua condição física e garantir que o plano seja adequado para você. Este chatbot oferece sugestões baseadas em informações fornecidas, mas não substitui a orientação profissional.
* **Diretrizes da OMS:** O plano gerado busca seguir as recomendações da Organização Mundial da Saúde, mas a interpretação e aplicação dessas diretrizes podem variar.

## ✍️ Autor
Liana Bernat
