################################################################################

# HYBRID DL-LLM FRAMEWORK FOR ATOPIC DISEASE PREDICTION

# Undergraduate Thesis - Sinam Afi Serwa Ametewee

# Ashesi University | Computer Science Department | 2026

################################################################################

# GITHUB REPOSITORY

# 

# Full code and documentation available at:

# https://github.com/sinaaa-aaam/Undergraduate_Thesis

################################################################################

# INSTALLATION INSTRUCTIONS

################################################################################

# STEP 1: CLONE THE REPOSITORY

# 

git clone https://github.com/sinaaa-aaam/Undergraduate_Thesis.git
cd Undergraduate_Thesis

# STEP 2: INSTALL PYTHON DEPENDENCIES

# 

pip install -r requirements.txt

# Alternatively, install manually:

pip install numpy pandas scikit-learn
pip install torch pytorch-tabnet
pip install tabpfn
pip install google-generativeai

# STEP 3: DOWNLOAD ISAAC DATASET

# 

# 1. Register at: https://datacatalogue.ukdataservice.ac.uk/studies/study/8131

# 2. Download ISAAC Phase III questionnaires for children aged 6-7 years

# 3. Place files in data/ directory:

# - isaac_core_questionnaire.csv

# - isaac_environmental_questionnaire.csv

# STEP 4: CONFIGURE GEMINI API KEY

# 

# Get free API key from: https://aistudio.google.com/app/apikey

# 

# For Google Colab:

# - Click the key icon (🔑) in left sidebar

# - Add secret: GEMINI_API_KEY

# - Enable “Notebook access”

# 

# For local Jupyter:

# - Create .env file: echo “GEMINI_API_KEY=your_key_here” > .env

################################################################################

# HOW TO RUN

################################################################################

# OPTION 1: GOOGLE COLAB (RECOMMENDED)

# 

# 1. Upload Undergraduate_Thesis.ipynb to Google Colab

# 2. Runtime → Change runtime type → GPU (optional, for faster training)

# 3. Runtime → Run all

# 4. Expected runtime: ~45 minutes

# OPTION 2: LOCAL JUPYTER NOTEBOOK

# 

jupyter notebook Undergraduate_Thesis.ipynb

# Then: Cell → Run All

################################################################################

# SYSTEM REQUIREMENTS

################################################################################

# Software:

# - Python 3.8 or higher

# - Jupyter Notebook or Google Colab

# - 8GB RAM minimum (16GB recommended)

# - GPU optional (speeds up TabNet training)

# Expected Runtime:

# - Data preprocessing: ~2 minutes

# - Model training (6 models total): ~40 minutes

# - LLM integration: ~1 minute per sample

################################################################################

# WHAT THIS SYSTEM DOES

################################################################################

# This hybrid DL-LLM framework:

# 

# 1. Trains 3 deep learning models (TabNet, TabPFN, MLP) on ISAAC data

# 2. Compares clinical-only vs clinical+environmental features

# 3. Demonstrates +4.4% AUC improvement from environmental data

# 4. Uses Gemini LLM to translate predictions into clinical recommendations

# 

# Key Results:

# - TabNet:  AUC 0.875 (ΔAUC +0.046)

# - TabPFN:  AUC 0.873 (ΔAUC +0.044)

# - MLP:     AUC 0.870 (ΔAUC +0.041)

# 

# Population Impact: 440 additional children correctly classified per 10,000

################################################################################

# PROJECT STRUCTURE

################################################################################

# Undergraduate_Thesis/

# ├── Undergraduate_Thesis.ipynb    # Main notebook (all experiments)

# ├── README.md                      # Detailed documentation

# ├── requirements.txt               # Python dependencies

# ├── USER_MANUAL.md                 # Comprehensive user guide

# ├── data/                          # ISAAC dataset (download separately)

# ├── models/                        # Saved models (generated after running)

# ├── results/                       # Experiment outputs

# └── figures/                       # Visualizations

################################################################################

# TROUBLESHOOTING

################################################################################

# Problem: ModuleNotFoundError

# Solution: pip install -r requirements.txt

# Problem: API key not recognized

# Solution: Add GEMINI_API_KEY to Colab Secrets or .env file

# Problem: Out of memory errors

# Solution: Use Google Colab Pro or reduce batch size in notebook

# Problem: Dataset not loading

# Solution: Verify CSV files are in data/ directory with correct filenames

################################################################################

# ADDITIONAL DOCUMENTATION

################################################################################

# For detailed instructions, see:

# - README.md (project overview)

# - USER_MANUAL.md (step-by-step guide with troubleshooting)

# - requirements.txt (complete dependency list)

# For questions or issues:

# - Open an issue: https://github.com/sinaaa-aaam/Undergraduate_Thesis/issues

# - Contact: Sinam Afi Serwa Ametewee (Ashesi University)

################################################################################

# LICENSE

################################################################################

# MIT License

# Copyright (c) 2026 Sinam Afi Serwa Ametewee

# See LICENSE file for full details

################################################################################

# END OF README

################################################################################
