# AI-Based Applications for Natural Language Understanding and Information Extraction

This repository contains two AI-based application focused on natural language understanding and information extraction:

## 1. Optical Text Analysis & Answer System

### Overview
A desktop application that extracts text from images, summarizes it, and allows users to ask questions based on the extracted content.

### Technologies Used
- **Python**
- **PyQt6**: GUI framework for building the desktop app.
- **Pytesseract**: OCR tool for extracting text from images.
- **Transformers (HuggingFace)**:
  - `google/pegasus-cnn_dailymail` for text summarization.
  - `distilbert-base-uncased` for question answering.
- **PIL (Pillow)**: For handling image processing.
- **gTTS**: Converts text to speech.

### How It Works
1. **Image Upload**: Users upload an image containing text.
2. **Text Extraction**: Pytesseract reads the image and extracts the textual content.
3. **Summarization**: The full text is summarized using the Pegasus model.
4. **Question Answering**: Users input questions which are answered using a DistilBERT-based QA model.
5. **Text-to-Speech**: Any text result can be converted to audio using Google Text-to-Speech.

### Requirements
Found in `requirements.txt`, including:
- `transformers`
- `pytesseract`
- `PyQt6`
- `Pillow`
- `gtts`

---
