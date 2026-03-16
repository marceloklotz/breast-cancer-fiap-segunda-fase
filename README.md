# 🏫👨‍💻 Tech Challenge - Pós Tech (8IADT) FIAP - Fase 2: Otimização de Diagnóstico de Câncer de Mama

Este repositório contém a solução para o Tech Challenge da Fase 2 da Pós-Tech em IA para Devs (FIAP - 8IADT). O projeto foca na evolução de modelos preditivos de diagnóstico médico utilizando Algoritmos Genéticos e Grandes Modelos de Linguagem (LLMs), conforme instruções contidas no PDF fornecido [(Tech Challenge - Fase 2.pdf)](https://github.com/marceloklotz/Breast-Cancer---Tech-Challenge-Fase-2/blob/main/8IADT%20-%20Fase%202%20-%20Tech%20challenge.pdf).

O notebook final do grupo foi incluído em:
https://github.com/marceloklotz/breast-cancer-fiap-segunda-fase/blob/main/FIAP_Fase_2.ipynb

## 📝 Descrição do Desafio

O objetivo principal é melhorar a precisão e a interpretabilidade dos modelos de diagnóstico desenvolvidos na fase anterior
. Para isso, implementamos:
Otimização de Hiperparâmetros: Uso de Algoritmos Genéticos para encontrar a configuração ideal do modelo
. Interpretabilidade via LLM: Integração com modelos de linguagem para gerar explicações humanizadas sobre os diagnósticos para profissionais de saúde

## 👥 Integrantes do grupo
Os membros do grupo são compostos pelos seguintes servidores da Secretaria de Segurança Pública do Distrito Federal (SSP/DF):

- Alexandre Natã Vicente (**rm370024**) (ale.n.vicente@gmail.com)
- Antônio Cláudio Almeida (**rm370052**) (antonioalmeida@gmail.com)
- Cyd Ferreira Rodrigues (**rm370004**) (cydnelson@gmail.com)
- David Catherink (**rm369997**) (d.catherinck@gmail.com)
- Marcelo Macedo Klotz (**rm370010**) (marceloklotz@gmail.com)

## 🎲 Base de dados

Utilizamos uma versão modificada do dataset Breast Cancer Wisconsin, que inclui atributos morfológicos de biópsias mamárias. Para **fins didáticos**, foram incorporados dados demográficos como idade e etnia.

- Base original:
https://github.com/marceloklotz/breast-cancer-fiap-segunda-fase/blob/main/FIAP_Fase_2.ipynb

- Dados gerados para fins didáticos:
https://raw.githubusercontent.com/marceloklotz/breast-cancer-fiap-segunda-fase/refs/heads/main/dados_demograficos_aleatorios_idade_etnia.csv

- Dados gerados pelo notebook contendo (prompts e respostas):
https://raw.githubusercontent.com/marceloklotz/breast-cancer-fiap-segunda-fase/refs/heads/main/fase2_llm_explanations.csv

## 🛠️ Implementação Técnica

### 🧬 Algoritmos Genéticos (GA)

Para otimizar os hiperparâmetros, o GA foi configurado com:
- Genes: Representação dos hiperparâmetros (ex: learning rate, profundidade de árvore).
- Operadores: Implementação de seleção, cruzamento (crossover) e mutação.
- Função Fitness: Baseada em métricas de desempenho como Recall e F1-Score, priorizando a redução de falsos negativos no contexto médico.

### 🤖 Integração com LLMs

Utilizamoo o GPT-4o mini, que é um modelo de inteligência artificial da OpenAI, projetado para ser uma versão rápida, leve e acessível (barata) do modelo principal para transformar resultados numéricos e estatísticos (SHAP/Feature Importance) em insights acionáveis.  Apesar de ser uma solução mais acessível é robusta o suficiente para o caso proposto.

- Prompt Engineering: Desenvolvimento de instruções específicas para garantir que as explicações sejam precisas e adequadas ao contexto clínico.

## 📒 Relatório técnico

O relatório técnico descreve o desafio proposto e a forma de exploração de dados adotada pelos membros do grupo, explicando as estratégias de pré-processamento e limpeza dos dados, os modelos avaliados e utilizados, os resultados obtidos, a interpretação do dados, além da aplicabilidade prática e as lições aprendidas durante o desenvolvimento da atividade acadêmica.

O download do relatório pode ser feito diretamente pelo seguinte link: 

- [https://github.com/marceloklotz/breast-cancer-fiap/blob/main/Tech%20Challenge%20-%20Fase%201.pdf](https://github.com/marceloklotz/breast-cancer-fiap/blob/main/Tech%20Challenge%20-%20Fase%201.pdf)

## 📽️ Vídeo explicativo

O vídeo explicativo sobre a metologia, resultados e notebook em execução foi disponbilizado a partir do seguinte link:

- [https://www.youtube.com/watch?v=8BE0_HIzjS8](https://www.youtube.com/watch?v=8BE0_HIzjS8)
