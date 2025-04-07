# 🧠 TAGAN: Text-Aware Generative Adversarial Network
Multimodal AI System for Text-Aware Image Generation and Enhancement

## 📌 Overview
TAGAN is a cutting-edge multimodal AI pipeline designed to generate, detect, understand, correct, and enhance text within images. The system intelligently processes AI-generated images containing textual content and ensures both visual fidelity and linguistic accuracy. This is achieved through a multi-layer architecture combining GANs, OCR, ML, and NLP.

🚀 Key Features
🎨 AI Image Generation using a generative model.

🔍 Text Detection & Classification using a custom-trained ML classifier.

📖 OCR & Text Extraction based on the ICDAR dataset.

🧠 Text Correction & Rephrasing using transformer models.

🧼 Text Removal from images while preserving background.

✍️ Text Reinsertion using matched font, size, and color.

🛠️ Image Enhancement: Sharpening, denoising, and detail preservation.

## 🧩 System Architecture
```
1. Text Prompt → Image Generation (GAN)
2. Text Detection → (ML Classifier)
3. OCR → Text Extraction (ICDAR)
4. Transformer → Text Understanding & Correction
5. Image Cleanup → Text Removal
6. Image Editing → Overlay Corrected Text
7. Final Output → Enhanced Image
```
## 🗂️ Dataset
* ICDAR 2013/2015: Used for OCR training and evaluation.

* Custom Dataset: Contains mixed real/generated images with and without text.

## 📁 Folder Structure:

```
├── training_images/
│   └── mixed images (text + no_text)
├── test_images/
│   └── mixed test data
```
## ⚙️ Technologies Used
* GANs (for image generation)
* Scikit-learn / XGBoost (for text/no-text classification)
* Tesseract / EasyOCR (for OCR)
* Transformers (Hugging Face) (for text correction)
* OpenCV / PIL / Diffusion Models (for text removal and reinsertion)
* PyTorch / TensorFlow (for model development)

## 🧪 Evaluation Metrics
* OCR Accuracy (WER/CER)
* Image Quality (PSNR, SSIM)
* BLEU Score (for text correction)
* Expert Visual Validation

## 🔐 Security & Robustness
* Noise filtering and adversarial robustness for real-world applications.
* Handles low-resolution, distorted, or noisy text images effectively.

## 📽️ Demo


##🧑‍💻 How to Run
```
# Clone the repo
git clone https://github.com/yourusername/TAGAN.git
cd TAGAN

# Install requirements
pip install -r requirements.txt

# Run the main pipeline
python main.py --image_path sample_images/ --prompt "Your image prompt here"
```
##💡 Future Work
* Integration with real-time video stream.
* Font/style transfer for dynamic text matching.
* Deployment as an interactive web app.

## 🤝 Contributions
Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

## 📜 License
MIT License. See LICENSE for more information.
