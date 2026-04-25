# 📊 Training Recommendation System

An interactive, data-driven HR analytics dashboard that analyzes employee skill gaps and recommends personalized training programs — built with Python and Streamlit.

---

## 🌟 Overview

Organizations often struggle to identify skill deficiencies across their workforce and assign the right training programs efficiently. This system automates that workflow by:

- Analyzing skill scores for each employee across multiple competency areas
- Detecting and highlighting skill gaps with color-coded severity indicators
- Recommending targeted training programs based on identified weaknesses
- Providing HR teams with interactive search, filter, and visualization tools for informed decision-making

> ✅ This project simulates a real-world **Training Analyst** workflow — combining data analysis, business insight delivery, and interactive dashboard design.

---

## 🚀 Features

- 📋 **Dataset Preview** — View the full employee skill dataset with ratings across competency areas
- 🔴🟠🟢 **Color-Coded Skill Gap Highlighting** — Red (critical), Orange (moderate), Green (strong)
- 🎯 **Automated Training Recommendations** — Maps each skill gap to a targeted training program
- 📊 **Training Demand Charts** — Bar charts showing the most in-demand training programs across the workforce
- 🔍 **Employee Search Tool** — Search by Employee ID or Name to view individual skill profiles
- 🏢 **Department-Wise Filtering** — Drill down by department to analyze team-level skill distributions
- 📈 **Interactive Visualizations** — Built with Plotly for dynamic, responsive charts

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Language | Python |
| Dashboard UI | Streamlit |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Plotly |
| Dataset | CSV (simulated employee data) |

---

## 📁 Project Structure

```
training-recommendation-system/
│
├── app.py                      # Main Streamlit application
├── data/
│   └── employee_skills.csv     # Employee skill dataset
│
├── utils/
│   ├── gap_analysis.py         # Skill gap detection logic
│   ├── recommender.py          # Training recommendation engine
│   └── visualizations.py      # Chart generation functions
│
├── requirements.txt            # Python dependencies
└── README.md
```

---

## ⚙️ Installation & Setup

### Prerequisites

- Python 3.7+
- pip

### 1. Clone the Repository

```bash
git clone https://github.com/adarshv15/training-recommendation-system.git
cd training-recommendation-system
```

### 2. Create a Virtual Environment (Recommended)

```bash
python -m venv venv

# Activate on Windows
venv\Scripts\activate

# Activate on macOS/Linux
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Dashboard

```bash
streamlit run app.py
```

Visit **http://localhost:8501** in your browser.

---

## 🧠 How It Works

```
Employee Dataset (CSV)
        │
        ▼
Data Loading & Preprocessing
(Pandas — clean, normalize skill scores)
        │
        ▼
Skill Gap Analysis
(Score < threshold → Flag as Gap)
        │
        ▼
Color-Coded Highlighting
(Red < 40 | Orange 40–60 | Green > 60)
        │
        ▼
Training Recommendation Mapping
(Each gap → Recommended training program)
        │
        ▼
Streamlit Dashboard
(Tables + Charts + Search + Filters)
```

---

## 📊 Dataset Schema

| Column | Description |
|--------|-------------|
| `Employee_ID` | Unique identifier for each employee |
| `Name` | Employee name |
| `Department` | Team or department |
| `Communication` | Skill score (0–100) |
| `Technical Skills` | Skill score (0–100) |
| `Leadership` | Skill score (0–100) |
| `Problem Solving` | Skill score (0–100) |
| `Time Management` | Skill score (0–100) |

> *(Columns vary based on your dataset — update accordingly)*

---

## 🎨 Dashboard Sections

### 1. 📋 Dataset Preview
Full tabular view of employee skill ratings with color-coded cells.

### 2. 🔴 Skill Gap Highlighting
Interactive table where cells are color-coded based on severity:
- 🔴 **Red** → Score below 40 (Critical gap — immediate training needed)
- 🟠 **Orange** → Score 40–60 (Moderate gap — improvement recommended)
- 🟢 **Green** → Score above 60 (Strong — no training required)

### 3. 📊 Training Demand Chart
Bar chart displaying which training programs are most in demand across the workforce — useful for HR budget planning.

### 4. 🔍 Employee Search Tool
Search any employee by ID or Name to instantly view:
- Their complete skill profile
- Identified gaps
- Recommended training programs

### 5. 🏢 Department Filter
Select a specific department to analyze team-level skill distributions and training priorities.

---

## 📦 requirements.txt

```
streamlit
pandas
numpy
matplotlib
plotly
```

---

## 📸 Screenshots

> *(Add your screenshots here)*

| Dataset Preview | Skill Gap Highlighting |
|---|---|
| ![Dataset](screenshots/dataset.png) | ![Gaps](screenshots/skill_gaps.png) |

| Training Demand Chart | Employee Search |
|---|---|
| ![Chart](screenshots/chart.png) | ![Search](screenshots/search.png) |

---

## 🔮 Future Improvements

- [ ] Upload custom employee CSV datasets via UI
- [ ] Export personalized training reports as PDF
- [ ] Integration with LMS (Learning Management Systems)
- [ ] ML-based skill gap prediction using historical training data
- [ ] Role-based access (HR Admin vs Manager view)

---

## 👨‍💻 Author

**Adarsha V**
- GitHub: [@adarshv15](https://github.com/adarshv15)
- Email: adarsh80737@gmail.com

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

*Built with 🐍 Python + Streamlit + Pandas + Plotly*
