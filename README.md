# Image Caption Generator

This project implements an image caption generation system using deep learning. It extracts image features using the VGG16 model and generates captions using an LSTM-based language model.

## Features
- Uses VGG16 for image feature extraction.
- Implements an LSTM-based model for caption generation.
- Processes and tokenizes text captions.
- Supports training on the Flickr8k dataset.

## Installation
### Prerequisites
Ensure you have Python and the following libraries installed:
```bash
pip install tensorflow numpy tqdm pickle
```

## Usage
1. **Dataset Setup**: Download and extract the [Flickr8k dataset](https://www.kaggle.com/datasets/adityajn105/flickr8k) and set the correct `base_dir` in the script.
2. **Feature Extraction**: Extract image features using VGG16.
3. **Train the Model**: Train the LSTM-based caption generator.
4. **Generate Captions**: Use the trained model to generate captions for new images.

## Model Architecture
- **Feature Extractor**: VGG16 pre-trained on ImageNet.
- **Language Model**: Embedding + LSTM layers.

## Results
After training, the model can generate captions describing images with reasonable accuracy.
BLEU: 0.059 & 0.061

