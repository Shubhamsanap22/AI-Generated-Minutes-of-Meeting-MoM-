# AI Minutes of Meeting Generator

## Project Overview

AI Minutes of Meeting is a Python-based application that processes meeting transcripts and generates structured meeting summaries.

The project combines Natural Language Processing (NLP), a BiLSTM deep learning model, and a Large Language Model (LLM) to identify important information from meeting conversations and organize it into meaningful meeting minutes.

The application works with text transcripts containing speaker labels, such as Speaker 1 and Speaker 2.

## Key Features

- **Transcript Processing:** Accepts meeting transcripts as text input.
- **Important Information Extraction:** Identifies relevant information from meeting conversations.
- **BiLSTM Classification:** Uses a trained BiLSTM model to classify sentences into categories.
- **AI-Based Summarization:** Uses Llama 3.2 through Ollama to generate structured summaries.
- **Meeting Insights:** Organizes extracted information into:
  - Key discussion points
  - Decisions
  - Action items
  - Important questions

## Technologies Used

- **Python** – Application development
- **PyTorch** – Deep learning model implementation
- **BiLSTM** – Sentence classification
- **NLP** – Text preprocessing and analysis
- **Ollama** – Local LLM execution
- **Llama 3.2 (3B)** – Meeting summarization

## Project Workflow

1. Provide a meeting transcript containing speaker-labelled conversations.
2. Process and prepare the transcript text.
3. Use the trained BiLSTM model to classify relevant sentences.
4. Pass the extracted information to the Llama 3.2 model.
5. Generate structured meeting minutes containing key points, decisions, and action items.

## Project Structure

```text
AI-Minutes-of-Meeting/
│
├── implementation.py
├── ai_miniproject.py
├── main.py
├── bilstm_best.pt
│
└── README.md
```

*Note: This is an illustrative structure based on the project files discussed. Update it if your actual repository contains additional files or folders.*

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/Shubhamsanap22/AI-Minutes-of-Meeting.git
```

### 2. Navigate to the project directory

```bash
cd AI-Minutes-of-Meeting
```

### 3. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 4. Install dependencies

Install the required Python packages based on the project's dependency list.

```bash
pip install torch numpy pandas
```

### 5. Set up Ollama

Install Ollama and download the Llama 3.2 model:

```bash
ollama pull llama3.2:3b
```

Make sure the Ollama service is running before executing the application.

### 6. Run the application

```bash
python main.py
```

*The execution command may need adjustment depending on your actual entry-point configuration.*

## Learning Outcomes

- Practical application of Natural Language Processing.
- Text preprocessing and sentence classification.
- Working with BiLSTM deep learning architectures.
- Integrating locally hosted Large Language Models.
- Combining traditional deep learning with Generative AI.
- Extracting structured information from unstructured meeting transcripts.

## Future Enhancements

- Add audio-to-text transcription.
- Develop a web-based user interface.
- Support exporting meeting minutes as PDF or DOCX.
- Improve summarization quality and action-item extraction.

## Author

**Shubham Sanap**

M.Tech Data Science | COEP Technological University

[GitHub](https://github.com/Shubhamsanap22) · [LinkedIn](https://www.linkedin.com/in/shubham-sanap-b7298224b/)

---

*An AI-based project exploring NLP, deep learning, and Generative AI for automated meeting documentation.*
