# 🤖 ChatPDF: Interaja com Documentos Usando IA

<img src="https://github.com/user-attachments/assets/a04c586a-a058-4976-a174-31e9f5484ace" alt="ChatPDF" style="width: 80%; max-width: 600px; display: block; margin: 0 auto;">

**ChatPDF** é uma aplicação poderosa desenvolvida em **Python** com **Streamlit**, que permite carregar e interagir com diferentes tipos de documentos (PDFs, CSVs, sites, vídeos do YouTube e arquivos de texto) utilizando modelos de linguagem avançados como **Groq** e **OpenAI**.

---

## 📖 Índice
- [🌟 Principais Funcionalidades](#principais-funcionalidades)
- [📦 Instalação](#instalação)
- [🚀 Como Usar](#como-usar)
- [🗂️ Estrutura do Projeto](#estrutura-do-projeto)
- [🧪 Testes](#testes)

---

## 🌟 Principais Funcionalidades

- **📂 Suporte a Diversos Tipos de Arquivos**:
  - PDFs
  - Arquivos CSV
  - Arquivos de texto
  - Conteúdo de sites
  - Transcrições de vídeos no YouTube
- **🧠 Assistentes de IA**:
  - Integração com modelos de linguagem baseados em Groq e OpenAI.
  - Respostas contextualizadas baseadas no conteúdo carregado.
- **💬 Memória de Conversa**:
  - Utiliza `ConversationBufferMemory` para manter o histórico de interações e oferecer uma experiência mais fluida.
- **💻 Interface Simples e Intuitiva**:
  - Desenvolvida com Streamlit, proporcionando facilidade de uso.

---

## 📦 Instalação

### Pré-requisitos
- **Python 3.7 ou superior** instalado no sistema.

### Passos para Instalação

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/LoboProgrammingg/Langchain-Site-Youtube-PDF-CSV-TXT.git
   cd Langchain-Site-Youtube-PDF-CSV-TXT
   ```

2. **Crie um ambiente virtual e ative-o**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```

3. **Instale as dependências**:
   ```bash
   pip install -r requirements.txt
   ```

4. **(Opcional) Dependências de Desenvolvimento**:
   Caso precise, instale as dependências para desenvolvimento:
   ```bash
   pip install -r requirements-dev.txt
   ```

---

## 🚀 Como Usar

1. **Execute a aplicação**:
   ```bash
   streamlit run home.py
   ```

2. **Na interface do Streamlit, você pode**:
   - Carregar diferentes tipos de documentos.
   - Escolher o modelo de linguagem desejado (Groq ou OpenAI).
   - Interagir com o assistente de IA para obter respostas baseadas no conteúdo carregado.

---

## 🗂️ Estrutura do Projeto

```plaintext
Langchain-Site-Youtube-PDF-CSV-TXT/
├── home.py               # Lógica principal da aplicação.
├── loaders.py            # Funções para carregar conteúdo de diferentes tipos de documentos.
├── requirements.txt      # Dependências necessárias para rodar o projeto.
├── requirements-dev.txt  # Dependências para desenvolvimento.
└── README.md             # Documentação do projeto.
```

### Arquivo `home.py`
- Contém a lógica principal da aplicação:
  - Configuração do Streamlit.
  - Carregamento de arquivos.
  - Inicialização de modelos de linguagem.
  - Exibição da interface do usuário.

### Arquivo `loaders.py`
- Funções para carregar conteúdo de diferentes fontes:
  - **carrega_site**: Carrega o conteúdo de uma URL.
  - **carrega_youtube**: Carrega a transcrição de vídeos do YouTube.
  - **carrega_csv**: Lê dados de arquivos CSV.
  - **carrega_pdf**: Extrai texto de arquivos PDF.
  - **carrega_txt**: Lê dados de arquivos de texto simples.

---

## 🧪 Testes

Execute testes automatizados para validar o funcionamento do projeto:

```bash
pytest tests/
```
