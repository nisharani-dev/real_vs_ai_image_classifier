# real_vs_ai_image_classifier# Real vs AI Image Classifier

This project implements a forensic pipeline to classify images as **real** (photographs) or **AI-generated** (fake) using handcrafted forensic features and a Random Forest classifier.

---

## Features Extracted

-Density Statistics

-Mean intensity of pixel values

-Standard deviation (std) of pixel values

-Sharpness / Focus Measure

-Laplacian variance (captures blurriness or sharpness differences in images)

-Edge & Texture Features

-Edge density (proportion of edge pixels, extracted via Canny or similar methods)

-Color Distribution 

---

## Requirements

- Python 3.x  
- OpenCV  
- scikit-image  
- PyWavelets  
- scikit-learn  
- joblib  
- tqdm  

Install dependencies with:

```bash
pip install -r requirements.txt

## Notes

- The current model is a Random Forest classifier trained on forensic features.  
- I look forward to improving accuracy and making the model compatible with more diverse AI-generated image datasets.  
- Feature extraction must remain consistent for prediction and retraining.
