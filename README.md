# Medical Prescription Digitization System (Ongoing)

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=flat&logo=python)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-orange?style=flat&logo=pytorch)](https://pytorch.org/)
[![HuggingFace](https://img.shields.io/badge/HuggingFace-Transformers-yellow?style=flat&logo=huggingface)](https://huggingface.co/)
[![Streamlit](https://img.shields.io/badge/Streamlit-App-FF4B4B?style=flat&logo=streamlit)](https://streamlit.io/)

End-to-end automated system that extracts and digitizes information from **printed** and **handwritten** medical prescriptions using advanced OCR and biomedical NLP — helping reduce medication errors by converting unstructured images into structured JSON output.

## 🎯 Project Highlights
- Achieves **90% accuracy** on printed text and **80%** on handwritten text (initial tests)
- Handles real-world challenges: noise, skew, varying handwriting
- Extracts key entities: drug names, dosages, frequencies, instructions
- Integrates external validation (RxNorm API)
- User-friendly prototype with **Streamlit** web interface

**Built as part of AI/ML internship at iHub Robotics + PG Diploma coursework.**

## 🛠️ Tech Stack
- **Core Language**: Python
- **Computer Vision/OCR**: OpenCV, TrOCR (fine-tuned transformer)
- **NLP/Entity Extraction**: spaCy + BioClinicalBERT, rule-based matchers
- **Deployment/UI**: Streamlit
- **Others**: PyTorch, Hugging Face Transformers, JSON output

## ✨ Features
- Image preprocessing (grayscale conversion, denoising, deskewing)
- OCR pipeline with fine-tuned TrOCR for high-accuracy text extraction
- Biomedical NER + rule-based parsing for structured medical data
- API integration for drug name validation
- Export results as clean JSON for further processing/integration

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- GPU recommended for faster inference (but works on CPU)

### Installation
```bash
# Clone the repository
git clone https://github.com/VidhyaES/medical-prescription-digitization-ocr-nlp.git
cd medical-prescription-digitization-ocr-nlp

# Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

# Install dependencies
pip install -r requirements.txt
