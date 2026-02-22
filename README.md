# 🛰️ Satellite Image Classification & Enhancement System


<div align="center">
  
  <br>
  <em>Automated satellite image analysis for environmental monitoring, urban planning, and disaster response</em>
</div>


## 🌟 **OVERVIEW**

This project presents an end-to-end **Satellite Image Classification and Enhancement System** developed by a team of 5 undergraduate students at Netaji Subhash Engineering College. The system automatically enhances low-quality satellite images and classifies them into 10 land cover types with **92.5% accuracy**.

**Key Highlights:**
- ✅ **Two-stage pipeline**: Enhancement + Classification
- ✅ **92.5% accuracy** on EuroSAT dataset (27,000 images)
- ✅ **150ms inference time** - suitable for real-time applications
- ✅ **Comprehensive documentation** with architecture diagrams

---

## 🎯 **PROBLEM STATEMENT**

Satellite imagery plays a critical role in:
- 🌲 Environmental monitoring (deforestation, glacier retreat)
- 🏙️ Urban planning (city expansion, infrastructure)
- 🌾 Agriculture (crop health, yield prediction)
- 🔥 Disaster management (floods, wildfires, landslides)

**However, raw satellite images suffer from:**
- 🌫️ Atmospheric haze and clouds
- 🌓 Uneven lighting and shadows
- 📉 Low contrast and poor visibility
- 📡 Sensor noise and distortions

These quality issues make accurate automated classification extremely challenging.

---
## 💡 **SOLUTION APPROACH**

Our solution combines traditional computer vision with deep learning:

## **Phase 1: Image Enhancement (OpenCV)**
```python
```
## **Enhancement pipeline that improved accuracy by 15%**
1. CLAHE → Local contrast enhancement
2. Gaussian Blur → Noise reduction  
3. Sharpening → Edge enhancement
4. Resize → Standardize to 224×224
## **Phase 2: Classification (EfficientNet-B0)**
- Transfer learning with ImageNet pretrained weights

- Fine-tuned for 10 land cover classes

- 92.5% accuracy with only 5.3M parameters


---

## 📊 **DATASET: EuroSAT**
We used the EuroSAT dataset - a benchmark for land use classification.

## **Attribute**           **Details**
- Source	          →      Sentinel-2 satellite
- Total Images	    →      27,000
- Classes	          →      10 land cover types
- Image Size	      →      64×64 to 256×256 pixels
- Spectral Bands	  →      13 (we used RGB)
- Coverage	        →      34 European countries

---

## **Class Distribution:**
## **Class**	                **Images**
- AnnualCrop	           →     3,000
- Forest	               →     3,000
- HerbaceousVegetation	 →     3,000
- Highway	               →     2,500
- Industrial	           →     2,500
- Pasture	               →     2,000
- PermanentCrop	         →     2,000
- Residential	           →     3,000
- River	                 →     2,500
- SeaLake	               →     3,500

---

## 🛠️ **TECHNOLOGIES USED**
### **Core Technologies**
### **Technology**              **Purpose**
- Python 3.8+	        →   Primary programming language
- PyTorch 1.9+	      →   Deep learning framework
- OpenCV 4.5+	        →   Image enhancement & processing
- EfficientNet-B0	    →   Classification model architecture   

---

## **Libraries & Tools**

- torch, torchvision  →  # Deep learning
- opencv-python       →  # Image processing
- numpy, pandas       →  # Data manipulation
- scikit-learn        →  # Metrics & preprocessing
- matplotlib          →  # Visualization
- tqdm                →  # Progress bars
- imageio             →  # Image I/O
- tensorboard         →  # Training logs


---

## **Development Environment**

- Google Colab (GPU training)

- VS Code (local development)

- Git/GitHub (version control)

---

## 🔍 **Image Enhancement**

- CLAHE: Local contrast enhancement revealing details in shadows

- Noise Reduction: Gaussian filtering to remove sensor noise

- Sharpening: Edge enhancement for better feature detection

- Before/After Comparison: Visual proof of improvement


---

## 🧠 **Intelligent Classification**

- Transfer Learning: Leverages ImageNet pretrained weights

- 10 Land Cover Classes: Comprehensive land type coverage

- Confidence Scoring: Each prediction includes confidence level

- Per-class Metrics: Detailed performance analysis

## 🌐 **Web Interface**

- Simple drag-and-drop upload

- Real-time classification

- Before/after enhancement display


## 📊 **Comprehensive Documentation**

- System architecture diagrams

- API specifications

- Training workflows

- Performance analysis reports

---


## 📈 **RESULTS & PERFORMANCE**
## **Overall Metrics**
### **Metric**       **Score**

- Accuracy	      →    92.5%
- Precision	      →    91.8%
- Recall	        →    92.1%
- F1-Score	      →    91.9%
- Inference Time  →	   150ms/image

## **Per-Class Accuracy**
### **Class**             **Accuracy**

- Forest	               →   95.2%
- SeaLake	               →   94.8%
- Residential	           →   93.1%
- AnnualCrop	           →   92.5%
- River	                 →   89.7%
- Industrial	           →   88.4%
- Pasture	               →   87.9%
- PermanentCrop	         →   86.5%
- HerbaceousVegetation	 →   85.8%
- Highway	               →   84.3%

## **Impact of Enhancement**

- Without Enhancement:   77.0% accuracy
- With Enhancement:      92.5% accuracy
- Improvement:           +15.5% 📈







