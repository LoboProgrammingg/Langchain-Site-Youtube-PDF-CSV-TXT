# ChatPDF
![Image](https://github.com/user-attachments/assets/a04c586a-a058-4976-a174-31e9f5484ace)

## Descrição do Projeto

O ChatPDF é uma aplicação desenvolvida em Python com Streamlit que permite carregar diferentes tipos de documentos (como PDFs, CSVs, sites, vídeos do YouTube e arquivos de texto) e interagir com assistentes de IA de diferentes provedores (Groq e OpenAI). O projeto utiliza a biblioteca `langchain` para orquestrar a interação entre o usuário e os modelos de linguagem.

## Funcionalidades

- **Carregamento de Arquivos:** Suporte para carregar documentos de sites, vídeos do YouTube, PDFs, arquivos CSV e arquivos de texto.
- **Assistentes de IA:** Integração com modelos de linguagem de diferentes provedores (Groq e OpenAI) para responder perguntas baseadas no conteúdo dos documentos carregados.
- **Memória de Conversa:** Utiliza `ConversationBufferMemory` para manter o histórico de conversação e melhorar a interação com o usuário.
- **Interface Simples:** Interface amigável e interativa desenvolvida com Streamlit.

## Instalação

### Pré-requisitos

- Python 3.7 ou superior

### Passos para Instalação

1. Clone o repositório:
   ```python
   git clone https://github.com/LoboProgrammingg/Langchain-Site-Youtube-PDF-CSV-TXT.git
   cd Langchain-Site-Youtube-PDF-CSV-TXT
   ```

2. Crie um ambiente virtual e ative-o:
   ```python
   python -m venv venv
   source venv/bin/activate  # No Windows, use `venv\Scripts\activate`
   ```

3. Instale as dependências:
   ```python
   pip install -r requirements.txt
   ```

4. (Opcional) Instale as dependências de desenvolvimento:
   ```python
   pip install -r requirements-dev.txt
   ```

## Uso

1. Execute a aplicação:
   ```python
   streamlit run home.py
   ```

2. Na interface do Streamlit, você pode:
   - Carregar diferentes tipos de documentos.
   - Selecionar o provedor e o modelo de linguagem desejado.
   - Interagir com o assistente de IA para obter respostas baseadas no conteúdo dos documentos carregados.

## Estrutura do Código

### home.py

Este arquivo contém a lógica principal da aplicação, incluindo:

- Carregamento de arquivos de diferentes tipos.
- Configuração e inicialização dos modelos de linguagem.
- Interface do usuário utilizando Streamlit.
- Funções para gerenciar a memória de conversação e exibir mensagens no chat.

### loaders.py

Este arquivo contém funções auxiliares para carregar conteúdo de diferentes tipos de documentos:

- **carrega_site:** Carrega o conteúdo de uma URL.
- **carrega_youtube:** Carrega o conteúdo de um vídeo do YouTube.
- **carrega_csv:** Carrega o conteúdo de um arquivo CSV.
- **carrega_pdf:** Carrega o conteúdo de um arquivo PDF.
- **carrega_txt:** Carrega o conteúdo de um arquivo de texto.

### requirements.txt

Lista de dependências necessárias para rodar a aplicação:

```python
streamlit==1.38.0
langchain==0.3.0
langchain-community==0.3.0
langchain-groq==0.2.0
langchain-openai==0.2.0
python-dotenv==1.0.1
beautifulsoup4==4.12.3
pypdf==5.0.0
unstructured==0.15.13
fake_useragent==1.5.1
youtube_transcript_api==0.6.2
```

### requirements-dev.txt

Lista de dependências para desenvolvimento:

```python
flake8==7.1.2
```

## Contribuição

Contribuições são bem-vindas! Sinta-se livre para abrir issues e pull requests.

## Licença

- Matheus Lobo Camara