# Sistema Multi-Agente para Análise de Perfil Estudantil com crewAI

## 🚀 Visão Geral

Este projeto implementa um sistema multi-agente que utiliza a biblioteca `crewAI` e modelos de linguagem da OpenAI para auxiliar no processo de identificação de universidades ideais para perfis específicos de estudantes.

A solução consiste em uma equipe de agentes de IA autônomos que colaboram para:

1.  Analisar dados de estudantes e universidades a partir de arquivos CSV.
2.  Criar um perfil detalhado para cada estudante.
3.  Identificar e recomendar as universidades mais compatíveis com o perfil de cada estudante.
4.  Gerar um relatório final com as recomendações.

---

## 🔨 Funcionalidades Principais

- **Análise de Perfil:** Agentes especializados em analisar os dados brutos dos estudantes para criar perfis enriquecidos, considerando suas notas, interesses e preferências.
- **Análise de Universidades:** Agentes que avaliam as universidades com base em seus cursos, localização, reputação e outros critérios relevantes.
- **Matching Inteligente:** Um agente gerente que orquestra a colaboração entre os outros agentes para cruzar os perfis dos estudantes com os das universidades e encontrar as melhores combinações.
- **Geração de Relatórios:** Criação de um relatório consolidado com a análise e as recomendações finais para cada estudante.

---

## ✔️ Técnicas e Tecnologias Utilizadas

- **Linguagem:** Programação Orientada a Objetos em Python
- **Framework de Agentes IA:** `crewAI`
- **Modelos de Linguagem (LLM):** GPT-4 (via API da OpenAI)
- **Manipulação de Dados:** Leitura e processamento de arquivos `.csv` com a biblioteca Pandas.
- **Gerenciamento de Dependências:** Pip e `requirements.txt`

---

## 🛠️ Abrir e Rodar o Projeto

Siga os passos abaixo para configurar e executar o projeto localmente.

### 1. Pré-requisitos

- Python 3.9+
- Conta na [OpenAI](https://openai.com/) com uma chave de API válida.

### 2. Baixe o Projeto

Clone este repositório para a sua máquina local:

```bash
git clone [https://github.com/SEU-USUARIO/crewai-sistema-universidade.git](https://github.com/SEU-USUARIO/crewai-sistema-universidade.git)
cd crewai-sistema-universidade
```

### 3. Crie e Ative o Ambiente Virtual

É uma boa prática usar um ambiente virtual para isolar as dependências do projeto.

**No Windows:**

```bash
python -m venv venv
venv\Scripts\activate
```

**No Mac/Linux:**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 4. Instale as Dependências

Com o ambiente virtual ativado, instale todos os pacotes necessários:

```bash
pip install -r requirements.txt
```

### 5. Configure a Chave de API

Para que os agentes possam funcionar, eles precisam da sua chave da OpenAI.

- Crie um arquivo chamado `.env` na pasta raiz do projeto.
- Dentro deste arquivo, adicione sua chave da seguinte forma:

```
OPENAI_API_KEY="SUA_CHAVE_DE_API_AQUI"
```

_Substitua "SUA_CHAVE_DE_API_AQUI" pela sua chave real._

### 6. Execute a Simulação

Para iniciar o processo, execute o script principal:

```bash
python main.py
```

O terminal mostrará o progresso dos agentes e, ao final, exibirá o relatório com as recomendações.

---
