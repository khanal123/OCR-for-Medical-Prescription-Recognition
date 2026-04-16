# Medical Prescription OCR using CRNN

## Project Overview
This project implements an Optical Character Recognition (OCR) system for extracting text from medical prescription images using a CRNN (Convolutional Recurrent Neural Network).

### The pipeline includes:
- Data preprocessing
- Vocabulary creation
- CRNN model training
- Evaluation using CER and WER
- Prediction visualization

---

## Requirements

Install the following Python packages:

```bash
pip install torch torchvision torchaudio
pip install opencv-python numpy pandas matplotlib scikit-learn pillow jiwer
```

---

## How to Run

1. Open terminal and navigate to the project folder:

2. Activate virtual environment (if used):  
   Mac/Linux: source venv/bin/activate  
   Windows: venv\Scripts\activate  

3. Launch Jupyter Notebook:

4. Open : Medical_Prescription_OCR_CRNN.ipynb

5. Run all cells from top to bottom.

---

## Model Details

- Model: CRNN (CNN + BiLSTM + CTC Loss)
- Input size: 512 × 64 grayscale images
- Optimizer: Adam
- Learning rate: 0.0001
- Batch size: 8
- Epochs: 10

---

## Evaluation Metrics

- CER (Character Error Rate)
- WER (Word Error Rate)

---

## Notes

- The model is trained on CPU due to compatibility limitations with Apple MPS.
- Target labels were simplified to "medicine + dosage" for better training performance.
- Some predictions may show repetitive patterns due to dataset limitations and sequence complexity.

---

## Authors

- Baradan Mainali  
- Suman Khanal  