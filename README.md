# EKYC System using Computer Vision

An advanced eKYC (Electronic Know Your Customer) system that automates identity verification using computer vision. This project incorporates OpenCV for image preprocessing, multiple OCR models for text extraction, DeepFace for facial recognition, and a MySQL database for user data management. Designed for modularity, accuracy, and ease of integration into enterprise applications.

---

## 📅 Project Duration

**November 2023 – April 2024**

---

## 🚀 Features

- **🖼️ Image Preprocessing**  
  Improved accuracy by 20% using:
  - CV2 Canny edge detection
  - Grayscale conversion
  - Gaussian blur
  - Adaptive OTSU thresholding
  - Contour detection for noise reduction

- **🔍 Optical Character Recognition (OCR)**  
  - Base CRNN model optimized for document OCR
  - Also tested: EasyOCR, PaddleOCR, Keras OCR, and Pytesseract
  - Fine-tuned for high precision on real-world ID documents

- **👤 Face Recognition**  
  - Integrated DeepFace for facial verification
  - Euclidean distance metric used for similarity comparison
  - Reduced false positives for reliable user authentication

- **⚙️ Modular Configuration Management**  
  - YAML-based configuration files
  - Enables modular programming and flexible model swapping

- **🗃️ Database Integration**  
  - MySQL used to securely store user data
  - Managed using SQLAlchemy ORM
  - Supports scalability and easy integration with third-party systems

---

## 🧰 Tech Stack

| Component              | Technology                      |
|------------------------|----------------------------------|
| Programming Language   | Python                          |
| Image Processing       | OpenCV (cv2)                    |
| OCR Models             | CRNN, EasyOCR, PaddleOCR, Keras OCR, Pytesseract |
| Face Recognition       | DeepFace                        |
| Database               | MySQL + SQLAlchemy              |
| Configuration          | YAML                            |
| Data Manipulation      | Pandas                          |

---

## 📁 Project Structure

ekyc-system/
├── configs/
│ └── config.yaml
├── preprocessing/
│ └── image_preprocessing.py
├── ocr/
│ ├── crnn_model.py
│ ├── easyocr_wrapper.py
│ ├── paddleocr_wrapper.py
│ └── ocr_utils.py
├── face_recognition/
│ └── deepface_module.py
├── database/
│ ├── models.py
│ └── db_manager.py
├── samples/
│ └── sample_id.jpg
├── main.py
├── requirements.txt
└── README.md

---

## 🛠️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ekyc-system.git
cd ekyc-system
pip install -r requirements.txt
database:
  host: localhost
  user: your_mysql_user
  password: your_mysql_password
  database: ekyc_db
python database/db_manager.py
python main.py

---

Let me know if you'd like to convert this project into a web app with Flask or React, or if you want a sample database schema or API documentation added!
