# Automating Text Recognition and Transliteration of Historical Documents with Convolutional-Recurrent Architectures

## Project Summary
Extracting text from centuries-old manuscripts and early printed works presents challenges that conventional OCR tools like Adobe Acrobat cannot handle. These tools excel at recognizing modern print but struggle with historical fonts and handwritten documents. This project focuses on developing a self-supervised AI model tailored for recognizing text in 17th-century Spanish printed sources using convolutional-recurrent architectures.

---

## Task: RenAIssance Project Evaluation for GSoC 2025 Candidates

### Objective
As part of the evaluation, I have designed an Optical Character Recognition (OCR) model built upon convolutional-recurrent architectures. I have developed this model from scratch and successfully applied it to the given dataset.

### Solution Notebook
The project is encapsulated in a Jupyter Notebook as .ipynb, making it easy to execute in Google Colab or a local Jupyter environment.

---

## Methodology & Implementation
To achieve accurate text recognition, I followed a structured and methodical approach:

### 1. In-Depth Research
I began by reviewing existing research on Optical Character Recognition (OCR) models, studying various methods and architectures to understand their effectiveness.

### 2. Preprocessing the Data
Ensuring the dataset was properly formatted was crucial for effective training. This involved cleaning, resizing, and structuring the input data.

### 3. Image Conversion
A custom Python function was developed to convert provided PDFs into images, preserving textual integrity for accurate recognition.

### 4. Splitting Multi-Page Documents
For better training efficiency, I separated double-page scans into individual pages, allowing the model to focus on isolated text instances.

### 5. Mapping Words to Images
To create a well-structured training set, I implemented a mapping mechanism that associates each word with its corresponding image section.

### 6. Detecting Text Boundaries
I employed the CRAFT model to detect bounding boxes around text regions, accurately segmenting words and lines for OCR processing.

### 7. Data Organization
To avoid misalignment in training, I devised a sorting algorithm that arranges text regions first vertically, then horizontally, ensuring proper sequencing.

### 8. Training the Model
Using a CNN-RNN architecture, I trained the OCR model with the Connectionist Temporal Classification (CTC) loss function to improve text recognition accuracy.

---

## Performance & Evaluation
### Training Dataset
A curated dataset was used to optimize model learning and generalization.

### Text Predictions
The model successfully extracted and recognized text from historical sources.

### CTC Loss Analysis
Training was monitored using CTC loss metrics to ensure optimal character recognition efficiency.

---

## Future Enhancements

### 1. Integrating Self-Supervised Learning & Transformers
Exploring self-supervised learning techniques and transformer-based architectures will enhance the model’s ability to recognize complex historical scripts.

### 2. Expanding the Dataset
Incorporating a more diverse set of historical documents will improve the model’s adaptability and accuracy across various fonts and writing styles.

### 3. Continuous Model Optimization
Further fine-tuning through hyperparameter optimization and architectural refinements will enhance accuracy and efficiency, ensuring robust OCR performance on historical texts.

---

This project strives to bridge the gap in existing OCR technology by developing an AI-driven solution tailored for historical document transliteration, facilitating better access to ancient texts and preserving cultural heritage.

