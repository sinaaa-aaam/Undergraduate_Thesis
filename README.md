# Hybrid DL-LLM Framework for Atopic Disease Prediction

**Undergraduate Thesis**  
**Sinam Afi Serwa Ametewee**  
Ashesi University | Computer Science Department | 2026  

---

# 🔗 Repository

Full code and documentation available here:  
https://github.com/sinaaa-aaam/Undergraduate_Thesis  

---

# ⚙️ Installation

## 1. Clone the Repository
```bash
git clone https://github.com/sinaaa-aaam/Undergraduate_Thesis.git
cd Undergraduate_Thesis
```

## 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### Alternatively (manual install):
```bash
pip install numpy pandas scikit-learn
pip install torch pytorch-tabnet
pip install tabpfn
pip install google-generativeai
```

---

# 📊 Dataset Setup (ISAAC)

1. Register here:  
   https://datacatalogue.ukdataservice.ac.uk/studies/study/8131  

2. Download:
   - ISAAC Phase III questionnaires (children aged 6–7)

3. Place files in the `data/` directory:

```
data/
├── isaac_core_questionnaire.csv
├── isaac_environmental_questionnaire.csv
```

---

# 🔑 API Configuration (Gemini)

Get a free API key:  
👉 https://aistudio.google.com/app/apikey  

## Google Colab
- Click 🔑 (Secrets) in sidebar  
- Add: `GEMINI_API_KEY`  
- Enable **Notebook access**

## Local Jupyter
```bash
echo "GEMINI_API_KEY=your_key_here" > .env
```

---

# ▶️ How to Run

## Option 1: Google Colab (Recommended)
1. Upload `Undergraduate_Thesis.ipynb`
2. Runtime → Change runtime → GPU (optional)
3. Runtime → **Run all**

⏱ Expected runtime: ~45 minutes  

---

## Option 2: Local Jupyter Notebook
```bash
jupyter notebook Undergraduate_Thesis.ipynb
```

Then: **Cell → Run All**

---

# 💻 System Requirements

## Software
- Python 3.8+
- Jupyter Notebook or Google Colab  

## Hardware
- Minimum: 8GB RAM  
- Recommended: 16GB RAM  
- GPU (optional, speeds up training)

## Runtime Estimates
- Data preprocessing: ~2 minutes  
- Model training (6 models): ~40 minutes  
- LLM integration: ~1 minute/sample  

---

# 🚀 What This System Does

This hybrid **Deep Learning + LLM framework**:

- Trains 3 models:
  - TabNet  
  - TabPFN  
  - MLP  

- Compares:
  - Clinical-only features  
  - Clinical + environmental features  

- Demonstrates:
  - **+4.4% AUC improvement** with environmental data  

- Uses Gemini LLM to:
  - Convert predictions into **clinical recommendations**

---

# 📈 Key Results

| Model   | AUC   | ΔAUC |
|--------|------|------|
| TabNet | 0.875 | +0.046 |
| TabPFN | 0.873 | +0.044 |
| MLP    | 0.870 | +0.041 |

**Population Impact:**  
➡️ ~440 additional children correctly classified per 10,000  

---

---

# 🛠 Troubleshooting

## ModuleNotFoundError
```bash
pip install -r requirements.txt
```

## API Key Not Working
- Ensure `GEMINI_API_KEY` is set correctly  
- Check Colab Secrets or `.env` file  

## Out of Memory Errors
- Use Google Colab (or Colab Pro)  
- Reduce batch size  

## Dataset Not Loading
- Confirm files exist in `data/`  
- Verify filenames match exactly  

---
 

---
