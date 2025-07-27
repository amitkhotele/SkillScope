# 📊 Student Technical Skills Analyzer & PDF Report Generator

This project analyzes technical skills of students based on a structured dataset and generates individual PDF reports that include:

- 📈 Radar Charts for Visual Analysis  
- 📋 Skill Gap Tables with Recommendations  
- ✅ Evaluation of Coding Skills, Projects, Certifications, and Online Presence

---

## 🚀 Features

- Load and clean data from Excel or CSV files  
- Analyze academic performance and technical capabilities  
- Automatically detect missing areas like competitive programming links or certifications  
- Generate radar charts showing 5 major skills  
- Export personalized PDF reports for each student

---

## 📁 Folder Structure

```
.
├── main.ipynb                 # Jupyter Notebook to run the analysis
├── student_data.xlsx          # Input sheet with student data
├── reports/                   # Folder where individual reports are saved
├── assets/                    # Radar charts are saved here temporarily
└── README.md
```

---

## 📥 Input Sheet Format (`student_data.xlsx`)

Ensure your Excel file contains the following columns:

| Column Name       | Description                                           |
|-------------------|-------------------------------------------------------|
| Name              | Full name of student                                  |
| BTech%            | Average BTech percentage till 6th sem                 |
| Languages         | Comma-separated programming languages                 |
| Projects          | Text list of projects with descriptions               |
| Certifications    | Comma-separated certifications                        |
| GitHub            | GitHub profile link                                   |
| LinkedIn          | LinkedIn profile link                                 |
| Portfolio         | Portfolio link                                        |
| CP                | Competitive programming profile link (LeetCode etc.)  |

---

## 🛠️ Requirements

Install all required libraries using:

```bash
pip install pandas matplotlib fpdf2 openpyxl
```

---

## 🧠 How It Works

1. **Data Cleaning**  
   Cleans special characters like `%`, handles missing values.

2. **Score Calculation**  
   Evaluates students on 5 dimensions:  
   - **Academics**  
   - **Coding Skills**  
   - **Projects**  
   - **Certifications**  
   - **Online Presence**  

3. **Radar Chart Generation**  
   Visualizes the above scores in a spider plot using `matplotlib`.

4. **Skill Gap Analysis**  
   Identifies missing or weak areas and gives smart recommendations.

5. **PDF Report Generation**  
   Each student's report includes:
   - Radar chart  
   - Skill gap table  
   - Recommendations  

---

## 📌 Example Report Output

- **Amit Khotele**
  - ✅ Strong Academics (80%+)
  - ✅ Knows Python, JavaScript
  - ✅ Projects in Web & AI
  - ❌ No Competitive Programming Profile
  - ⚠️ Medium Certifications

✅ **Download:** `reports/Amit_Khotele_Report.pdf`

---

## 📤 Output Example (PDF)

<img width="635" height="618" alt="Screenshot 2025-07-27 231529" src="https://github.com/user-attachments/assets/f586c4ec-041b-47e0-92e7-88524281055e" />

---

## 📈 Customizations

- Adjust scoring weights in `calculate_scores()`  
- Modify recommendations in `skill_gap()`  
- Add student photo or more insights if needed

---

## 📬 Future Improvements

- Add AI-based project recommendations  
- Auto-email reports to students  
- Build web interface for uploading sheets & downloading reports

---

## 👨‍💻 Author

**Amit Khotele**  
