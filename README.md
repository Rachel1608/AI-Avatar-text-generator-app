# AI Avatar Text Generator using NLP & Streamlit

[![Streamlit App](https://img.shields.io/badge/Streamlit-Live%20App-red?logo=streamlit)](https://ai-avatar-9ul5z5wxjubkhennpmwaqf.streamlit.app/)

## Demo Video

![Streamlit Demo](images/ai_avatar_appdemo.gif)


This project demonstrates the **end-to-end application of Natural Language Processing (NLP)** and **web app development** to build an **AI-powered document understanding system**. The application extracts text from uploaded documents, performs **Named Entity Recognition (NER)**, and generates a structured summary that can be used for **AI avatars, storytelling systems, or intelligent assistants**.


## Problem Statement

Unstructured documents such as PDFs and Word files contain valuable information, but extracting meaningful insights manually is time-consuming. This project automates:

- Text extraction from documents
- Identification of important entities (people, places, dates, organizations)
- Generation of concise summaries for AI-driven applications


## Key Skills Demonstrated

- Natural Language Processing (NLP)
- Named Entity Recognition (NER)
- Text preprocessing and cleaning
- Streamlit-based web application development
- Handling unstructured document data


## Technologies & Tools

- **Python**
- **Streamlit** – Interactive web UI
- **SpaCy** – NLP and NER
- **PyPDF2** – PDF text extraction
- **python-docx** – DOCX file handling
- **Regex** – Text preprocessing


##  Project Workflow (Code Logic Explained)

###  File Upload Interface

Users upload PDF or DOCX documents through a Streamlit-based UI.

###  Text Extraction

- PDF files are processed using PyPDF2
- DOCX files are processed using python-docx

###  Text Preprocessing

- Converts text to lowercase
- Removes special characters
- Normalizes spacing for NLP accuracy

###  Named Entity Recognition (NER)

SpaCy’s `en_core_web_sm` model extracts:

- **Characters (PERSON)**
- **Locations (GPE)**
- **Dates (DATE)**
- **Organizations (ORG)**

###  AI Avatar Summary Generation

Extracted entities are used to generate a structured summary suitable for:

- AI avatar narration
- Storytelling systems
- Intelligent assistants


##  Output

- Raw extracted text
- Cleaned and normalized text
- Categorized named entities
- Automatically generated summary


##  How to Run

```bash
pip install streamlit spacy PyPDF2 python-docx
python -m spacy download en_core_web_sm
streamlit run app.py
```


## Future Enhancements

- Integrate transformer-based models (BERT) for advanced summarization
- Add sentiment analysis for richer AI avatar responses
- Support additional file formats (TXT, HTML)
  
