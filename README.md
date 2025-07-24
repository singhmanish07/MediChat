# MediChat :hospital:

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Python](https://img.shields.io/badge/Python-3.12%2B-blue)

An end-to-end medical chatbot powered by Generative AI. Ask health-related questions and get informed, accurate answers in real-time.

![image](https://github.com/user-attachments/assets/65324687-98dd-4bca-b84e-2059e4157a24)

---

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
  - [Clone Repository](#clone-repository)
  - [Create & Activate Conda Environment](#create--activate-conda-environment)
  - [Install Dependencies](#install-dependencies)
  - [Configure Environment Variables](#configure-environment-variables)
- [Usage](#usage)
  - [Indexing Documents](#indexing-documents)
  - [Running the App](#running-the-app)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- :brain: Medical AI Assistant with **Gemini 2.0 Flash** LLM
- :mag_right: Semantic search using **HuggingFace** embeddings & **Pinecone** vector DB
- :gear: Built with **Python 3.12**, **Flask**, and **LangChain**
- :art: Modern glassmorphism UI with real-time interactions
- :warning: Built-in safety checks for emergency responses

## Tech Stack

- **Language & Framework**: Python 3.12, Flask
- **AI & LLM**: LangChain, Google Gemini 2.0 Flash
- **Embeddings**: HuggingFace Transformers (`all-MiniLM-L6-v2`)
- **Vector DB**: Pinecone
- **Frontend**: HTML5, Bootstrap 5, jQuery, CSS Glassmorphism

| Category            | Technologies                          |
|---------------------|---------------------------------------|
| Backend             | Python 3.12, Flask, LangChain         |
| AI/LLM              | Google Gemini 2.0 Flash, HuggingFace  |
| Vector Database     | Pinecone                              |
| Frontend            | Bootstrap 5, CSS Glassmorphism        |

## Prerequisites

- [Conda](https://docs.conda.io/en/latest/) installed
- :snake: Python 3.12+
- :key: API Keys:
  - Google Gemini API Key
  - Pinecone API Key

## Installation

### Clone Repository

```bash
git clone https://github.com/singhmanish07/MediChat.git
cd MediChat
```

### Create & Activate Conda Environment

```bash
conda create -n medichat python=3.12 -y
conda activate medichat
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Environment Variables

Create a `.env` file in the project root and add:

```ini
PINECONE_API_KEY="YOUR_PINECONE_API_KEY"
GEMINI_API_KEY="YOUR_GOOGLE_API_KEY"
```

> **Note**: Keep your keys secret. Do not commit `.env` to version control.

## Usage

### Indexing Documents

Generate and upload embeddings for your documents:

```bash
python store_index.py
```

### Running the App

```bash
python app.py
```

Open your browser at `http://localhost:8080` to start chatting.

## Contributing

1. Fork the repo
2. Create a feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add feature'`)
4. Push and open a Pull Request

## License

MIT © [https://singhmanish.vercel.app/](https://singhmanish.vercel.app/)