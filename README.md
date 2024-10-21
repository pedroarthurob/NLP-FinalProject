# ENEM Study Assistant - Projeto de Disciplina

Este projeto foi desenvolvido como parte da disciplina de Processamento de Linguagem Natural (PLN), com foco em técnicas avançadas de geração aumentada por recuperação (RAG) e agentes de IA para criar um assistente de estudo para o ENEM.

## Objetivo do Projeto

O assistente tem como objetivo auxiliar estudantes a se prepararem para o ENEM, permitindo a criação de planos de estudo personalizados, sugerindo questões diárias, e analisando tópicos mais recorrentes nas provas anteriores.

## Como Utilizar o Projeto no Google Colab

### 1. Abrir o Projeto no Google Colab
- Faça o download do arquivo `.ipynb` deste repositório ou clone diretamente o repositório no [Google Collab](https://colab.research.google.com/drive/1vPzVFd_4Pzla2VpOrHmimOmIn4OV688K?usp=sharing) utilizando o seguinte comando:
  ```bash
  !git clone https://github.com/pedroarthurob/NLP-FinalProject.git
  ```
  
### 2. Configurar a API Key da OpenAI
Após clonar o repositório, será necessário configurar a chave da API da OpenAI para permitir que o sistema interaja com o modelo LLM. Insira o seguinte comando no início do notebook:
```python
import os
os.environ["OPENAI_API_KEY"] = "sua-chave-api"
```
Substitua `"sua-chave-api"` pela sua chave de acesso.

### 3. Execução do Notebook
Depois de configurar sua chave de API, basta executar o notebook. As dependências necessárias serão instaladas automaticamente durante a execução, o upload dos arquivos de provas e gabaritos será realizado e o projeto estará pronto para uso.

### 4. Execução das Funcionalidades
Após configurar as dependências e realizar o upload dos arquivos, o usuário poderá interagir com as seguintes opções no menu do projeto:

- **Criar Plano de Estudos**: O sistema fará a análise das questões e gabaritos de acordo com o ano e os tópicos escolhidos, gerando um plano de estudos personalizado com base nas notas do usuário.
- **Pesquisar Tópico(s)**: O sistema permitirá que o usuário busque tópicos específicos, retornando uma análise detalhada sobre cada tema, incluindo materiais de estudo relevantes e informações sobre a frequência de aparição nas provas.
- **Elaborar Estratégias**: O sistema criará estratégias de estudo que ajudarão a otimizar o aprendizado, sugerindo questões diárias e assuntos para revisão com base nas notas fornecidas pelo usuário.

## Funcionalidades

O projeto oferece três funcionalidades principais:

### 1. Criar Plano de Estudos
Permite ao usuário elaborar um plano de estudos personalizado, levando em consideração suas notas e os tópicos que deseja focar.

### 2. Pesquisar Tópico(s)
O usuário pode pesquisar um ou mais tópicos específicos do ENEM. O sistema retornará uma análise detalhada sobre cada tema, incluindo materiais de estudo relevantes e informações sobre a frequência de aparição nas provas.

### 3. Elaborar Estratégias
Com base nas notas informadas pelo usuário, o sistema cria estratégias de estudo que ajudam a otimizar o aprendizado, priorizando áreas que precisam de mais atenção.

## Menu Interativo

O projeto oferece várias funcionalidades que podem ser acessadas por meio de um menu interativo. O usuário pode escolher entre as seguintes opções:

1. **Criar Plano de Estudos**
   
2. **Pesquisar Tópico(s)**
   
3. **Elaborar Estratégias**

4. **Sair**

### Exemplos de Uso:

**1. Criação de Plano de Estudos**
   
   Ao escolher a opção "Criar plano de estudos", o usuário insere suas notas nas disciplinas de linguagens, humanas, natureza, matemática e redação.

   ```bash
   Escolha uma opção (1-4): 1
   Informe suas últimas notas obtidas em linguagens, humanas, natureza, matemática e redação
   (utlize '.' para as notas e as separe por vírgula): 703.4, 731.5, 804.9, 897,5, 960
   ```

   O sistema processa as notas e gera um plano de estudo personalizado com base nas informações fornecidas.

**2. Pesquisa de Tópico(s)**

   O usuário pode optar por pesquisar tópicos específicos que deseja estudar.
   
   ```bash
   Escolha uma opção (1-4): 2
   Por favor, informe os tópicos que você gostaria de estudar, separados por vírgula: Funções Matemáticas, História da Arte
   ```

   O agente processa a solicitação e retorna:
  
   Lista de materiais de estudo
   Frequência de aparição dos temas nas últimas provas do ENEM
   Sugestões de vídeos e exercícios
  
**3. Criação de Estratégias**

   O usuário pode elaborar estratégias de estudo, informando suas notas nas diferentes disciplinas.


   ```bash
   Escolha uma opção (1-4): 3
   Informe suas últimas notas obtidas em linguagens, humanas, natureza, matemática e redação
   (utlize '.' para as notas e as separe por vírgula): 703.4, 731.5, 804.9, 897,5, 960
   ```
   O sistema cria um plano de estratégias baseado nas notas informadas e nas disciplinas que o usuário precisa focar.

## Testando a Aplicação

Após a instalação das dependências e a configuração da chave API do OpenAI, você pode testar as funcionalidades principais seguindo os passos abaixo:

1. Clone ou realize o download do arquivo no Google Collab.
2. Execute as células e siga as instruções interativas para acessar os diferentes recursos.
3. Teste cada funcionalidade (criar plano de estudos, pesquisar tópico(s), elaborar estratégias).

### Observação:

- Para garantir a melhor performance, recomenda-se ter uma chave API com permissões suficientes e atentar-se ao limite de requisições por minuto (RPM) da API.

## Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## Contato

Caso tenha dúvidas ou sugestões, entre em contato:

- **Nome**: Pedro Arthur de Oliveira Barreto
- **Email**: pedroarthurbarreto28@gmail.com
- **LinkedIn**: [pedroarthurbarreto](https://www.linkedin.com/in/pedro-arthur-barreto/)

Sinta-se à vontade para contribuir com o projeto ou compartilhar feedback!
