# 🚜 Agriculture ML Project: Crop Production Prediction & Crop/Weed Detection

This repository contains a two-part machine learning project:
1. **Crop Production Prediction** using historical cost and variety data (ML with XGBoost)
2. **Crop and Weed Detection** using deep learning object detection (YOLOv5)

---

## 📁 Project Structure
```
Agriculture-ML-Project/
├── crop_prediction/
│   ├── crop_model.py             # Train and evaluate XGBoost model
│   ├── streamlit_app.py         # Dashboard for crop production prediction
│   ├── data/                    # Dataset files (e.g., crop_production.csv)
│   └── model/                   # Trained model (.pkl)
│
├── weed_detection/
│   ├── train.py                 # YOLOv5 training script
│   ├── detect.py                # Streamlit interface for crop/weed detection
│   ├── data/                    # Dataset (images + YOLO labels)
│   ├── cropweed.yaml            # YOLO dataset config file
│   └── best.pt                  # Trained model weights
│
├── Final_Report_Agriculture.pdf # Internship final report
├── README.md
└── requirements.txt             # Required libraries
```

---

## 🚀 Features
### ✅ Crop Production Prediction
- Input: Cost of cultivation, crop, state, variety
- Output: Expected production (quintals)
- Trained using **XGBoost**
- Deployed with **Streamlit dashboard**

### ✅ Crop & Weed Detection
- Input: Image with plants
- Output: Object detection boxes for crop/weed
- Trained with **YOLOv5** (custom annotated dataset)
- Deployable via **Streamlit** or edge devices

---

## 🔧 Setup Instructions
### Install Dependencies
```bash
pip install -r requirements.txt
```

### Run Crop Prediction Dashboard
```bash
cd crop_prediction
streamlit run streamlit_app.py
```

### Run Crop & Weed Detection
```bash
cd weed_detection
yolo detect.py  # or use python detect.py
```

### Train YOLOv5 (optional)
```bash
cd weed_detection
yolo train.py
```

---

## 📊 Datasets
- **Crop Prediction**: CSV file containing crop, state, cost, and yield
- **Weed Detection**: Custom image dataset in YOLO format (2 classes: crop, weed)

---

## 📚 Documentation
- [Final_Report_Agriculture.pdf](./Final_Report_Agriculture.pdf)
- Dataset structure, training config, and model files are documented in each module

---

## 📌 Author
**Kaushal Prasad** – B.Tech CSE Student, Parul University  
> Project developed during internship with Upskill Campus & UCT (The IoT Academy)

---

## 🌐 Links
- 🔗 GitHub Repo: [github.com/kaushalprasad21/upskillcampus](https://github.com/kaushalprasad21/upskillcampus)
- 📄 Report: [Final Report (PDF)](./Final_Report_Agriculture.pdf)

---

## 📝 License
This project is licensed for academic and demonstration purposes only.

---

**End of README**
