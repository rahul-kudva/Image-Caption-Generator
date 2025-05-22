# Image Captioning with VGG16 and LSTM

This project generates captions for images using a deep learning model that combines VGG16 for visual feature extraction and LSTM for sequence modeling, trained on the Flickr8k dataset.

## Dataset

- Dataset: Flickr8k

## Pipeline

1. Mount Google Drive and unzip Flickr8k dataset
2. Clean and tokenize captions, add start/end tokens
3. Extract 4096-d image features using pretrained VGG16
4. Tokenize captions, pad sequences, and prepare inputs
5. Build a model combining image features and LSTM-based caption generation
6. Train for 6 epochs with categorical crossentropy
7. Generate and evaluate captions using BLEU score

## Output

- Trained model: trained_lstm_model.keras
- BLEU score evaluation
- Sample predictions on test images

## Requirements

Python 3.x, TensorFlow/Keras, NLTK, NumPy, Matplotlib, Pillow

## How to Run

1. Upload dataset and pretrained VGG16 weights to Google Drive
2. Run each step in the Colab notebook to preprocess, train, and evaluate
