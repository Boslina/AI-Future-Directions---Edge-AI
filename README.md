# AI Edge and IoT Smart Agriculture Prototypes

This repository contains two AI assignments demonstrating **Edge AI** and **AI-driven IoT simulations**.

---

## Task 1: Edge AI Prototype (Garbage Classification)

### Objective
Develop a lightweight image classification model to recognize recyclable items and simulate deployment on edge devices using TensorFlow Lite.

### Tools
- TensorFlow / TensorFlow Lite  
- Google Colab (simulation of Raspberry Pi / Edge device)  
- Python (Pandas, NumPy, scikit-learn)  

### Dataset
- Garbage Classification dataset containing images of recyclable items:
  - Classes include: `glass`, `metal`, `paper`, `cardboard`, `trash`, etc.
- Dataset preprocessing includes:
  - Removing missing images
  - Lowercasing filenames
  - Creating train/validation/test splits

### Workflow
1. **Load and clean data**: ensure all images exist and labels are consistent.  
2. **Create TensorFlow datasets** for efficient training.  
3. **Build MobileNetV2 lightweight model** with transfer learning.  
4. **Train model** with early stopping and checkpointing.  
5. **Evaluate model** and generate:
   - Test accuracy
   - Confusion matrix
   - Classification report  
6. **(Optional)** Convert trained model to TensorFlow Lite for Edge AI deployment.  

### Key Features
- Automatic handling of missing files  
- Lightweight architecture suitable for edge devices  
- Ready for TFLite conversion  

---

## Task 2: AI-Driven IoT Smart Agriculture

### Objective
Simulate a smart agriculture system using IoT sensors and AI to predict crop yields.

### Sensors Simulated
- Soil moisture  
- Temperature (air/soil)  
- Humidity  
- Light intensity (lux)  
- pH  
- Electrical Conductivity (EC)  
- CO2 levels  

### AI Model
- **Random Forest Regressor** predicts crop yield (kg/ha) based on sensor readings  
- Input features: sensor data  
- Output: predicted crop yield  
- Model trained on simulated sensor dataset  

### Workflow
1. **Simulate sensor readings** for multiple crops.  
2. **Generate synthetic crop yield** based on sensor data.  
3. **Train AI model** (Random Forest Regressor).  
4. **Evaluate model** with mean squared error.  
5. **Simulate real-time IoT reading** and predict yield.  

### Data Flow Diagram
Sensors -> IoT Device -> Data Preprocessing -> AI Model -> Prediction -> Dashboard/Alerts

---

## How to Run

1. Clone the repository:
```bash
git clone <repo-url>
cd <repo-name>
Open EdgeAI_Garbage_Classification.ipynb in Google Colab or local Jupyter Notebook.

Run Task 1 workflow:

Load dataset

Train MobileNetV2 model

Evaluate and optionally convert to TFLite

Run Task 2 workflow:

Simulate IoT sensor readings

Train Random Forest model

Predict crop yield for new sensor data

Dependencies

Python >= 3.8

TensorFlow >= 2.12

Pandas

NumPy

scikit-learn

Matplotlib (optional for visualizations)

Author

Abosede Bamidele
