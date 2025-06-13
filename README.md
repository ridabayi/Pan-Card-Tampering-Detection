
# 🛡️ PAN Card Tampering Detection using SSIM & OpenCV

An advanced AI-powered image forensics tool to detect tampering in PAN card documents. This project leverages **Structural Similarity Index (SSIM)** and **OpenCV** to highlight manipulated areas between an original and a potentially forged image.

---

## 📌 Overview

In the age of digital document submissions, tampering and forgery of identity cards like PAN cards is a serious concern. This project uses image comparison techniques to:

- Detect tampering in scanned or photographed PAN cards
- Highlight altered regions using contour detection
- Offer a fully visual, interpretable output for human review

---

## 🧠 Methodology

The pipeline compares two images:
1. **Original PAN card**
2. **Possibly tampered version**

It performs:
- Grayscale conversion
- **SSIM (Structural Similarity Index)** comparison
- Thresholding and contour detection
- Bounding box annotation over forged regions

---

## 🧬 Tech Stack

| Tool         | Purpose                              |
|--------------|--------------------------------------|
| `Python 3.10+` | Core language                     |
| `OpenCV`     | Image loading, processing, visualization |
| `scikit-image` | SSIM computation               |
| `imutils`    | Contour handling helper              |
| `matplotlib` | Image plotting                       |
| `NumPy`      | Numerical operations                 |

---

## 🖼️ Visual Example

![Output Imagel](https://github.com/ridabayi/Pan-Card-Tampering-Detection/blob/main/output.png)

---

## 🗂️ Project Structure

```
pan_card_tampering/
├── pan_card_tampering/
│   ├── image/
│   │   ├── original.png
│   │   └── tampered.png
├── PAN_Card_Tampering_SSIM_Advanced.ipynb
├── README.md
├── requirements.txt
└── static/
    └── demo/
        ├── original.png
        ├── tampered.png
        └── output.png
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/pan-card-tampering-detection.git
cd pan-card-tampering-detection
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Add your images

Place your images in:

```
pan_card_tampering/image/original.png
pan_card_tampering/image/tampered.png
```

### 4. Run the notebook

```bash
jupyter notebook PAN_Card_Tampering_SSIM_Advanced.ipynb
```

---

## ✅ How It Works

- `compare_ssim` computes perceptual differences between original and tampered images.
- Significant changes are extracted using adaptive thresholding.
- Contours are drawn to highlight those regions.

---

## 🛠️ Future Enhancements

- ✅ Add real-time inference via Flask API
- 🔍 Integrate OCR (e.g., Tesseract) for text tampering detection
- 🤖 Extend with CNN-based image forgery classification
- 🌍 Deploy to cloud (Render, HuggingFace Spaces, etc.)

---

## 👨‍💻 Author

**Rida Bayi**  
🧠 Data Scientist · 🧰 MLOps Engineer · 🔐 AI for Cybersecurity  
[LinkedIn](https://linkedin.com/in/ridabayi) · [GitHub](https://github.com/ridabayi)

---

## 📄 License

This project is licensed under the **MIT License** – feel free to use and modify.
