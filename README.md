
# ENEM Study Assistant - Projeto de Disciplina

Este projeto foi desenvolvido como parte da disciplina de Processamento de Linguagem Natural (PLN), com foco em técnicas avançadas de geração aumentada por recuperação (RAG) e agentes de IA para criar um assistente de estudo para o ENEM.

## Objetivo do Projeto

O assistente tem como objetivo auxiliar estudantes a se prepararem para o ENEM, permitindo a criação de planos de estudo personalizados, sugerindo questões diárias, e analisando tópicos mais recorrentes nas provas anteriores.

## Instalação

1. **Clonar o repositório**

   ```bash
   git clone https://github.com/seu-usuario/enem-study-assistant.git
   cd enem-study-assistant
   ```

2. **Instalar as dependências**

   Use o `pip` para instalar as dependências listadas no arquivo `requirements.txt`:

   ```bash
   pip install -r requirements.txt
   ```

3. **Configurar a chave da API do OpenAI**

   O projeto utiliza a API do OpenAI para realizar as operações de NLP e agentes. Você precisará de uma chave API para rodar o projeto.

   - Acesse [OpenAI API](https://platform.openai.com/) para criar uma chave.
   - Crie um arquivo `.env` na raiz do projeto com o seguinte conteúdo:

   ```bash
   OPENAI_API_KEY=your_openai_api_key
   ```

## Funcionalidades

O projeto oferece três funcionalidades principais:

### 1. Pesquisa de Tópicos do ENEM

Permite ao usuário pesquisar tópicos específicos do ENEM, retornando os conteúdos de estudo mais relevantes, vídeos e frequência dos tópicos nas últimas provas.

### 2. Criação de Planos de Estudo

Baseado no tempo disponível do usuário e nos tópicos de interesse, o assistente gera um plano de estudos personalizado, distribuindo os temas ao longo dos dias até a prova.

### 3. Sugestão de Questões Diárias

A partir dos tópicos de estudo diários, o assistente sugere questões de provas anteriores para reforçar o aprendizado.

## Menu Interativo

O projeto oferece várias funcionalidades que podem ser acessadas por meio de um menu interativo. O usuário pode escolher entre as seguintes opções:

1. **Pesquisar Tópico do ENEM**: Permite ao usuário pesquisar um tópico específico do ENEM, e o agente retornará uma análise detalhada sobre o tema, incluindo conteúdos de estudo e relevância.
   
2. **Criar Plano de Estudo**: Gera um plano de estudo personalizado, considerando o tempo disponível e os tópicos que o usuário deseja cobrir.

3. **Sugestão de Questões Diárias**: Com base no histórico e nas preferências do usuário, o agente sugere questões para o estudo diário, ajudando na prática e revisão dos conteúdos.

### Exemplos de Uso:

**1. Pesquisa de Tópico**
   
   Ao escolher a opção "Pesquisar Tópico", o usuário insere um tema (ex: *Funções Matemáticas*), e o sistema retornará materiais de estudo relevantes, tópicos mais recorrentes nas provas anteriores e links úteis.

   ```bash
   Digite o tópico que deseja estudar: Funções Matemáticas
   ```

   O agente processa a solicitação e retorna:
   - Lista de materiais de estudo
   - Frequência de aparição do tema nas últimas provas do ENEM
   - Sugestões de vídeos e exercícios

**2. Criação de Plano de Estudo**

   O usuário pode gerar um plano de estudos personalizado ao informar quantos dias ele possui para se preparar e quais os assuntos de maior prioridade.

   ```bash
   Digite o número de dias disponíveis para estudar: 30
   Digite os principais assuntos que deseja focar: Matemática, Física, Química
   ```

   O sistema gerará um plano de estudo balanceado, distribuindo os tópicos ao longo dos dias disponíveis.

**3. Sugestão de Questões Diárias**

   Para auxiliar na prática, o sistema pode sugerir um conjunto de questões diárias relacionadas ao tópico do dia.

   ```bash
   Sugestões de questões para o dia:
   - Questão 1: Funções Matemáticas - ENEM 2018
   - Questão 2: Probabilidade - ENEM 2019
   ```

## Estrutura de Pastas

A estrutura de pastas do projeto foi organizada para facilitar a localização dos arquivos e modularizar as funcionalidades:

```
enem-study-assistant/
│
├── data/                     # Provas e gabaritos do ENEM organizados por ano
│   ├── provas/
│   └── gabaritos/
│
├── notebooks/                # Notebooks de implementação do projeto
│   ├── agent_research.ipynb   # Implementação dos agentes de busca e sugestão
│   └── training_plan.ipynb    # Notebook para criação de planos de estudo
│
├── scripts/                  # Scripts auxiliares do projeto
│   └── pdf_extraction.py      # Script de extração de dados dos PDFs
│
├── requirements.txt          # Arquivo com as dependências do projeto
├── README.md                 # Arquivo atual (documentação do projeto)
└── LICENSE                   # Licença do projeto
```

## Testando a Aplicação

Após a instalação das dependências e a configuração da chave API do OpenAI, você pode testar as funcionalidades principais seguindo os passos abaixo:

1. Abra um dos notebooks na pasta `notebooks/`.
2. Execute as células e siga as instruções interativas para acessar os diferentes recursos.
3. Teste cada funcionalidade (pesquisa de tópicos, plano de estudo, sugestão de questões).

### Observação:

- Para garantir a melhor performance, recomenda-se ter uma chave API com permissões suficientes e atentar-se ao limite de requisições por minuto (RPM) da API.

## Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## Contato

Caso tenha dúvidas ou sugestões, entre em contato:

- **Nome**: Pedro Arthur de Oliveira Barreto
- **Email**: pedroarthurbarreto28@gmail.com
- **LinkedIn**: [Seu LinkedIn]([https://linkedin.com/in/seu-perfil](https://www.linkedin.com/in/pedro-arthur-barreto/))

Sinta-se à vontade para contribuir com o projeto ou compartilhar feedback!
