# Automating Text Recognition and Transliteration of Historical Documents with Convolutional-Recurrent Architectures

## Project Overview
Transliterating text from historical documents is a complex challenge that modern OCR tools, such as Adobe Acrobat, struggle to address. While these tools work well on contemporary printed material, they fail to extract text from older printed sources and handwritten manuscripts. This project aims to develop a self-supervised AI model capable of recognizing text in 17th-century Spanish printed documents using convolutional-recurrent architectures.

---

## Task Details: RenAIssance Project Evaluation for GSoC 2025 Applicants

### Task Description
As part of the evaluation, I have designed a model based on convolutional-recurrent architectures for Optical Character Recognition (OCR). Over the past two weeks, I have built this model from scratch and successfully implemented it on the provided dataset.

### Solution Notebook
The solution is a standalone Jupyter Notebook, ensuring easy execution in Google Colab or a local Jupyter environment.

---

## Approach & Methodology
To tackle this challenge, I followed a structured approach:

### 1. Research & Understanding
I started by exploring various research papers and articles on Optical Character Recognition models to gain a comprehensive understanding of their underlying principles.

### 2. Data Preprocessing
Proper data preprocessing was essential to ensure that the input format adhered to the required specifications. This included cleaning and structuring the dataset for optimal model performance.

### 3. Image Generation
Using Python, I developed a function to generate images from the provided PDF files, ensuring accurate text representation.

### 4. Page Splitting
To enhance the model’s ability to recognize text, I split double-sided pages into single-sided ones, improving training efficiency.

### 5. Word-to-Image Mapping
A crucial step in training was mapping each word from the document to its corresponding image, creating a structured training dataset.

### 6. Bounding Box Detection
Leveraging the CRAFT model, I implemented a bounding box detector to accurately locate and extract words from images.

### 7. Data Sorting
To prevent mismatches during training, I implemented a sorting algorithm that arranged images vertically, grouped similar values, and then sorted them horizontally.

### 8. Model Training
The CNN-RNN model was trained using the preprocessed dataset, employing the CTC (Connectionist Temporal Classification) loss function to optimize performance.

---

## Model Performance & Evaluation
### Training Dataset
A structured dataset was generated specifically for training the model.

### Predictions
The trained model successfully predicted text from the dataset.

### CTC Loss
The training process was monitored using the CTC loss metric, ensuring effective optimization for character recognition.

---

## Future Improvements

### 1. Implementing Self-Supervised Learning & Transformer Models
To further enhance text recognition accuracy, incorporating self-supervised learning techniques and transformer architectures can provide robust representations of input data.

### 2. Expanding the Training Dataset
Enriching the dataset with more historical documents and diverse writing styles will help the model generalize better and improve accuracy across different document formats.

### 3. Model Fine-Tuning & Optimization
Continuous refinement of the model architecture through hyperparameter tuning and architectural adjustments will further enhance OCR accuracy and efficiency. Regular evaluations on various historical documents will provide insights for additional improvements.

---

This project aims to bridge the gap in OCR technology by developing an AI-powered solution for historical document transliteration, ensuring better accessibility to centuries-old printed works.

