title: WiDS Datathon 2026 Presentation Template

class: title-slide

# WiDS Datathon 2026  
## Project Presentation

---

# 🔍 Problem Statement
- Wildfires are not only environmental disasters but also major economic disruptors
- Existing systems are fragmented: fire risk, economic data, and policies are disconnected
- Vulnerable communities are the most affected but the least informed

---

# 📁 Data Overview
- **Primary source:** Watch Duty dataset (~62,000 wildfire events, ~1,200 fire perimeters)  
- **Supplementary data:**
  - Sociodemographic → U.S. Census Bureau  
  - Economic → BLS, USDA  
  - Climate → NASA POWER, Open-Meteo  
  - Documents → policies, insurance, news (scraped corpus)  
- **Key variables:**
  - Climate → temperature, humidity, drought index, wind  
  - Economic → income, poverty rate, employment  
  - Demographic → population density, education, insurance  
- Data unified at **county level + multi-temporal resolution**

---

# 🛠️ Data Cleaning & Preprocessing
- Harmonization across **spatial (county-level)** and **temporal scales (weekly, monthly, yearly)**  
- Handling missing values (e.g., removing unreliable regions like Connecticut)  
- Feature engineering to build:
  - Exposure indicators  
  - Economic fragility metrics  
  - Sociodemographic vulnerability features  
- Normalization and dimensionality reduction (PCA)  
- Text preprocessing + filtering for document corpus  

---

# 📊 Exploratory Data Analysis
- Identified **heterogeneity across counties** in vulnerability patterns  
- Observed mismatch between:
  - High fire exposure  
  - High economic vulnerability  
- Key findings:
  - Some high-risk areas recover faster → resilience effect  
  - Some moderate-risk areas suffer more → hidden vulnerability  
- Spatial analysis revealed **clusters of high-risk + low-recovery capacity regions**

---

# 🧠 Modeling Approach
- **Unsupervised learning:**
  - K-means clustering → identify vulnerability profiles  
  - PCA → dimensionality reduction for economic/demographic indexes  
- **Climate modeling:**
  - Neural networks / autoencoders for pattern extraction  
- **WRVI (core model):**
  - Composite index:
    - Climate (50%)  
    - Economic (35%)  
    - Demographic (15%)  
- **Hybrid RAG system:**
  - Knowledge Graph (structured data)  
  - Document RAG (policies, reports)  
  - Hybrid + What-if reasoning  


---

# ⚙️ Model Evaluation
- WRVI evaluated using:
  - RMSE vs wildfire burn probability baseline  
- RAG system evaluated with:
  - Response time  
  - Semantic relevance  
  - Confidence scoring  
- Validation approach:
  - Benchmark vs existing indexes (e.g., CDC SVI)  
  - Qualitative validation through interpretability  

---

# 📈 Visualizing Results
- County-level **WRVI heatmaps (0–100 scale)**  
- Clustering visualizations (economic / demographic / climate profiles)  
- Interactive dashboard:
  - Map + chatbot interface  
- RAG outputs:
  - Evidence-based answers grounded in data + documents 

---

# 💡 Key Insights
- Risk is not just **where fires occur**, but **who cannot recover**  
- Economic fragility is a **stronger differentiator than exposure alone**  
- Data fragmentation is the real bottleneck, not data scarcity  
- Hybrid RAG enables:
  - Faster decision-making  
  - Explainable AI outputs  
- Unexpected finding:
  - Moderate-risk counties can be more vulnerable than extreme-risk ones 


---

# 🚀 Future Work
- Move from **county-level → census tract / granular data**  
- Improve document coverage in low-fire regions  
- Integrate real-time data streams  
- Expand to other disasters:
  - Floods, hurricanes, earthquakes  
- Build partnerships with:
  - Government agencies  
  - NGOs  
  - Insurance providers  

---

# 🧾 Summary & Reflections
- Successfully built a **multi-source, AI-driven decision system**  
- Shifted paradigm:
  - From reactive → proactive resilience  
- Learned:
  - Importance of data integration  
  - Responsible AI design in high-stakes environments  
  - Real-world constraints (data, ethics, scalability)  
- Biggest win:
  - Turning fragmented data into **actionable intelligence**  

---

# 💕 Thank You!
- Questions?
