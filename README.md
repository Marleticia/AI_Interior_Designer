# AI_Interior_Designer
Este repositório contém o código-fonte de um projeto desenvolvido como parte da 3º Edição da Imersão IA da Alura. Se trata de um Agente de IA para design de interiores usando Google Gemini.


🏡 Seu Agente de Design de Interiores e Planejamento com IA 🛋️

Descrição do Projeto

Este projeto é um agente de conversação desenvolvido em Python utilizando a API do Google Gemini. Ele foi criado como parte da [Nome da Imersão] com o objetivo de explorar o uso de modelos de linguagem grande (LLMs) para auxiliar pessoas no processo de design de interiores e planejamento de espaços residenciais.

O Agente oferece funcionalidades como:
- Condução de um briefing interativo para entender as necessidades e o estilo do usuário.
- Geração de sugestões de design e palavras-chave para busca de referências visuais online.
- Ajuda na otimização de espaços específicos (armários, closets, cantos) com base em medidas fornecidas.
- Suporte básico na interpretação textual de elementos em plantas de arquitetura.

Funcionalidades Implementadas

* **Briefing Conversacional:** O Agente guia o usuário através de perguntas para coletar informações essenciais sobre o projeto de design.
* **Sugestões de Design & Referências:** Com base no briefing, o Agente oferece ideias e orienta o usuário sobre onde buscar inspiração visual online.
* **Otimização de Espaço:** O usuário pode fornecer medidas e o Agente sugere layouts e soluções de organização para otimizar o espaço.
* **Ajuda com Plantas (Texto-base):** O Agente auxilia na compreensão de símbolos e medidas de plantas a partir da descrição textual do usuário, com ressalvas sobre as limitações.
* **Interface Interativa:** Implementada diretamente no Google Colab usando `ipywidgets` para facilitar a interação e demonstração.

Tecnologias Utilizadas

* Python
* Google Generative AI API (Modelo Gemini, via `google-generativeai`)
* Google Colab (Ambiente de Desenvolvimento e Execução)
* ipywidgets (Criação da Interface Gráfica no Notebook)

Como Rodar o Projeto no Google Colab

1.  **Obtenha sua API Key do Google AI Studio:**
    * Vá para o [Google AI Studio](https://aistudio.google.com/).
    * Crie ou acesse seu projeto.
    * Na navegação lateral, encontre a opção para obter sua API Key. Copie a chave.
2.  **Abra o Notebook no Google Colab:**
    * Faça o download deste arquivo `.ipynb` do GitHub.
    * Vá para o [Google Colab](https://colab.research.google.com/).
    * Clique em "Arquivo" > "Fazer upload de notebook" e selecione o arquivo que você baixou.
3.  **Configure sua API Key de Forma Segura:**
    * No Colab, vá no menu "Ambiente de execução" > "Ver segredos" (ou clique no ícone da chave 🔑 na barra lateral esquerda).
    * Clique em "+ Novo segredo".
    * No campo "Nome", digite **exatamente** `GOOGLE_API_KEY`.
    * No campo "Valor", cole a sua chave da API do Google AI Studio.
    * Certifique-se que o toggle ao lado está ativo para que o notebook tenha acesso a este segredo.
4.  **Execute as Células em Ordem:**
    * Execute a primeira célula para instalar as bibliotecas necessárias (`google-generativeai` e `ipywidgets`).
    * Execute a célula que configura a API Key.
    * Execute a célula que inicializa o modelo Gemini, inicia o chat e envia o prompt inicial (esse prompt configura o comportamento do Agente).
    * Execute a célula que define e exibe a interface interativa com `ipywidgets`.
5.  **Interaja com o Agente:** Use a caixa de texto e o botão que aparecerão na saída da última célula para conversar com seu Agente de Design!

Estrutura do Notebook

O notebook está organizado nas seguintes seções:
- Instalação de Bibliotecas
- Configuração da API e Inicialização do Agente
- Lógica do Agente (Prompt Engineering Detalhado)
- Interface de Usuário com ipywidgets

Nota de Segurança Importante

**NUNCA COLOQUE SUA API KEY DIRETAMENTE NO CÓDIGO FONTE OU EM ARQUIVOS QUE SERÃO COMPARTILHADOS PUBLICAMENTE NO GITHUB.** A forma correta e segura de usar chaves de API em ambientes como o Colab é através do recurso de Segredos do Colab (como instruído acima) ou utilizando variáveis de ambiente em outros contextos.

