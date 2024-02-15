# Image-captioning-VGG16

This repository contains the implementation of an image captioning system using a deep learning model that combines a Convolutional Neural Network (CNN) encoder and a Transformer-based decoder.

# Overview
The project uses a CNN encoder (based on InceptionV3) to extract features from images, and a Transformer-based decoder to generate captions. The model is trained on a subset of the MS COCO dataset.
# Getting Started
# Prerequisites
- Python 3.8 or later
- TensorFlow 2.4 or later
- NumPy
- Pandas
- Matplotlib
- Pillow
# Installation
Clone the repository and install the required packages:

bash
Copy code
- git clone https://github.com/sahu1shivani/image-captioning-VGG-16.git
- cd image-captioning
- pip install -r requirements.txt
# Model Architecture
The model architecture consists of:

- CNN Encoder: A modified InceptionV3 model that extracts features from images.
- Transformer Encoder Layer: Applies layer normalization, dense layers, and multi-head attention to the encoder input.
- Embeddings: Combines token embeddings with position embeddings.
- Transformer Decoder Layer: Includes multi-head attention layers (for self-attention and encoder-decoder attention), layer normalization, and feed-forward networks.
- ImageCaptioningModel: The main model that combines the CNN encoder, transformer encoder, and decoder.
