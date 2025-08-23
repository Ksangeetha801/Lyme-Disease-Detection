# Image Similarity Classifier (MobileNetV2 + Cosine Similarity)

This project classifies a test image as **POSITIVE** or **NEGATIVE** by comparing its features with reference datasets:
- **your_images/** → positive samples
- **other_images/** → negative samples

It uses a pre-trained **MobileNetV2** model (from TensorFlow/Keras) to extract deep features and applies **cosine similarity** for classification.

---

## 🚀 Workflow
1. Extract deep features of positive and negative images using MobileNetV2.
2. Extract features of the test image.
3. Compute cosine similarity between test image and dataset images.
4. Compare **mean similarity** and classify.

---

## 📂 Dataset
- Place positive samples inside `data/your_images/`
- Place negative samples inside `data/other_images/`
- Place test images inside `data/test_samples/`

👉 If dataset is large, upload it to Google Drive or provide a link in this section.

---

## 🛠️ Installation
Clone the repo and install dependencies:
```bash
git clone https://github.com/your-username/image-similarity-classifier.git
cd image-similarity-classifier
pip install -r requirements.txt
