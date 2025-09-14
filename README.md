# Diabetic-Retinopathy
# Hybrid Deep Learning Framework for Diabetic Retinopathy Detection

## 📌 Project Overview
Diabetic Retinopathy (DR) is a major complication of diabetes that can lead to blindness if not detected early. Traditional diagnosis requires expert ophthalmologists to review retinal fundus images, which is time-consuming and limited in scalability.  

This project presents a **hybrid deep learning model** that integrates:
- **EfficientNetB0 (CNN)** → extracts fine-grained local features like microaneurysms and hemorrhages.  
- **Vision Transformer (ViT)** → captures global dependencies and structural patterns across retinal images.  

By combining **10% EfficientNet + 90% Vision Transformer**, the model achieves high accuracy in DR severity classification.  

An interactive **web application** (Flask backend + React frontend) is also developed, allowing users to upload retinal images and receive real-time predictions of DR severity.

---

## ✨ Key Features
- Hybrid CNN + Transformer architecture for **robust DR detection**  
- **APTOS 2019 Blindness Detection Dataset** used for training & evaluation  
- Supports classification into **5 severity levels**:
  - 0 → No_DR  
  - 1 → Mild  
  - 2 → Moderate  
  - 3 → Severe  
  - 4 → Proliferative_DR  
- Data preprocessing with **augmentation, normalization, and class balancing**  
- Evaluation using **Accuracy, Precision, Recall, F1-score, and AUC**  
- Flask-React **web interface** for real-time predictions  

---

## 📊 Results
| Dataset | Accuracy | Precision | Recall | F1-Score | AUC |
|---------|----------|-----------|--------|----------|-----|
| Labeled Retinal Images | 84.80% | 80.65% | 80.54% | 80.59% | 85.44% |
| APTOS Dataset | **87.29%** | 84.12% | 82.28% | 83.18% | 89.34% |

- Best-performing model: **90% ViT + 10% EfficientNetB0**  
- Demonstrated **better generalization and less overfitting** with APTOS dataset  

---

## 🛠️ Tech Stack
- **Deep Learning**: PyTorch / TensorFlow  
- **Model Backbone**: EfficientNetB0 (CNN) + Vision Transformer (ViT)  
- **Backend**: Flask  
- **Frontend**: React.js  
- **Deployment**: Local/Server hosting with real-time prediction support  

---

## 📂 Project Structure
