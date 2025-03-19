# Pic2Text

## Overview
Pic2Text is an AI-powered image captioning system that converts images into meaningful text descriptions. Using deep learning techniques, it analyzes visual content and generates captions that accurately describe the image. This project leverages CNNs for feature extraction and LSTMs for sequence generation.

## Features
- **Automated Image Captioning** – Converts images into text-based descriptions.
- **Deep Learning-Based** – Uses CNN and LSTM models for accurate caption generation.
- **Pre-Trained Models** – Supports models like InceptionV3, ResNet, or custom-trained architectures.
- **Custom Training** – Train with your own dataset for domain-specific applications.
- **Multiple Output Formats** – Export captions in JSON, TXT, or integrate with APIs.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Pic2Text.git
   cd Pic2Text
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Download pre-trained models (if applicable) and place them in the `models/` directory.

## Usage
1. Run the script with an image:
   ```bash
   python caption.py --image sample.jpg
   ```
2. For batch processing:
   ```bash
   python batch_caption.py --folder images/
   ```
3. API Integration (Flask-based):
   ```bash
   python app.py
   ```
   Access the API at `http://localhost:5000/caption`

## Model Details
- **Encoder**: Uses a Convolutional Neural Network (CNN) to extract features from the image.
- **Decoder**: Uses an LSTM network to generate sequential captions from the extracted features.
- **Attention Mechanism**: Enhances caption accuracy by focusing on relevant parts of the image.

## Dataset
- Supports **MS-COCO**, **Flickr8k**, and **Flickr30k** datasets.
- Custom datasets can be added following the `data/` format.

## Example Output
**Input/Output Image:**
![Screenshot 2025-03-19 171918](https://github.com/user-attachments/assets/70e1f301-b6f5-4e7b-bafe-7710fcc3c4d4)



**Generated Caption:**
```
A dog sitting on the grass with a ball in front of it.
```

## Future Enhancements
- Improve caption accuracy with transformer-based models.
- Add multilingual support.
- Integrate with mobile applications.



