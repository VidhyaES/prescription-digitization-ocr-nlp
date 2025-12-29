# Prescription Digitization System (Ongoing)

End-to-end AI system that extracts and digitizes information from printed/handwritten medical prescriptions using OCR and biomedical NLP.

## Features
- Image preprocessing (grayscale, denoising, deskewing) with OpenCV
- OCR with fine-tuned TrOCR → 90% printed / 80% handwritten accuracy
- Entity extraction (drugs, dosage, frequency) using BioClinicalBERT + spaCy
- API validation with RxNorm
- Streamlit web prototype for user testing

## Tech Stack
- Python, OpenCV, PyTorch, Hugging Face Transformers
- spaCy, BioClinicalBERT, Streamlit

## Installation
```bash
git clone https://github.com/VidhyaES/prescription-digitization-ocr-nlp.git
cd prescription-digitization-ocr-nlp
pip install -r requirements.txt
streamlit run app.py
