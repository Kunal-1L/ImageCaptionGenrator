# Image Caption Generation

## Overview
This project implements an Image Caption Generation model using deep learning techniques, specifically leveraging CNNs and RNNs with an Encoder-Decoder architecture. The model is trained on the Flickr8k dataset to generate meaningful captions for images.

### Key Components:
1. **CNN (VGG16)** - Extracts high-level image features.
2. **RNN (LSTM)** - Generates sequential text descriptions based on image features.
3. **Tokenization** - Maps words to numeric tokens for input processing.
4. **BLEU Score Evaluation** - Measures the quality of generated captions.

## Dataset
The model is trained using the **Flickr8k dataset**, which consists of:
- 8,000 images
- 40,000 captions (5 captions per image)

## Training Details
- **Feature Extraction:** The VGG16 model (pre-trained on ImageNet) extracts image features.
- **Caption Processing:** Tokenization, padding, and sequence processing of captions.
- **Model Training:** Training on paired image-caption data using an Encoder-Decoder framework.

## Evaluation Metrics
The model is evaluated using **BLEU Score**, a standard metric for text generation tasks.

### BLEU Scores Achieved:
- **BLEU-1:** 0.543852
- **BLEU-2:** 0.316825

## Results
The model successfully generates captions that describe images accurately, achieving a BLEU-1 score of **0.543852** and a BLEU-2 score of **0.316825**.

## Future Improvements
- Use **Transformer-based models** like ViT + GPT for better captions.
- Train on **larger datasets** like MS-COCO for improved performance.
