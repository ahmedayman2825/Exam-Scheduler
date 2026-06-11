# 📅 ExamSync — Intelligent Exam Timetabling System

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter&logoColor=white" />
  <img src="https://img.shields.io/badge/NetworkX-Graph%20Coloring-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge" />
</p>

<br/>

## 📖 Overview

**ExamSync** is a constraint-based exam scheduling system that automatically generates conflict-free exam timetables for academic institutions. Built on top of **graph coloring theory**, it models courses as nodes and student enrollment overlaps as edges — then assigns time slots (colors) such that no two conflicting exams share the same slot.

The system takes student–course enrollment data as input, constructs a conflict graph, applies a greedy graph coloring algorithm, and outputs a complete, optimized timetable. Visualization tools and an optional Streamlit dashboard make results easy to interpret and present.

Whether you're managing a small department or a full university exam period, ExamSync eliminates manual scheduling headaches and ensures zero student conflicts.

<br/>

---

## ✨ Features

- **Conflict Detection** — Automatically identifies which courses share enrolled students and cannot be scheduled simultaneously.
- **Graph-Based Modeling** — Represents the scheduling problem as a graph coloring problem using NetworkX for robust, mathematically sound solutions.
- **Greedy Coloring Algorithm** — Efficiently assigns the minimum number of time slots needed to resolve all conflicts.
- **Conflict Graph Visualization** — Renders an interactive visual of the course conflict graph using Matplotlib, color-coded by assigned time slot.
- **Timetable Export** — Outputs the final schedule as a structured Pandas DataFrame, ready for export or further processing.
- **Scalable Input Handling** — Accepts enrollment data via CSV or manual input through the notebook interface.

<br/>

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Language | Python 3.8+ |
| Notebook Environment | Jupyter Notebook |
| Graph Modeling & Algorithm | NetworkX |
| Data Manipulation | Pandas, NumPy |
| Visualization | Matplotlib |

<br/>

---

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/ahmedayman2825/Exam-Scheduler.git
cd Exam-Scheduler
```

### 2. (Recommended) Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

<br/>

---

## 💡 Usage

### Jupyter Notebook

Launch the notebook to run the full scheduling pipeline interactively:

```bash
jupyter notebook Exam_Timetabling_System.ipynb
```

Inside the notebook, you can:
- Define or import your student–course enrollment data.
- Run the conflict detection and graph coloring cells step by step.
- View the conflict graph and the final generated timetable.


---

## 📁 Folder Structure

```
Exam-Scheduler/
│
├── Exam_Timetabling_System.ipynb   # Main notebook: full scheduling pipeline
├── requirements.txt                # Python dependencies
├── .gitignore                      # Git ignore rules
└── README.md                       # Project documentation
```

<br/>

---

## 👥 Contributors

 **Ahmed Ayman**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/eng-ahmed-ayman/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/ahmedayman2825)

Contributions are welcome! Feel free to open an issue or submit a pull request.

<br/>

---

## 🔭 Future Improvements

- **Room & Capacity Constraints** — Factor in room availability and seating capacity when assigning slots.
- **Multi-Day Scheduling** — Extend the model to distribute exams across a configurable number of days with daily slot limits.
- **Invigilator Assignment** — Auto-assign invigilators to exam slots based on availability and workload constraints.
- **CSV / Excel Upload UI** — Allow direct file uploads through the Streamlit dashboard without editing the notebook.
- **Export to PDF / Excel** — One-click export of the final timetable to printable or shareable formats.
- **Soft Constraint Optimization** — Incorporate preferences such as avoiding back-to-back exams for students or prioritizing certain courses for morning slots.
- **REST API** — Expose the scheduling engine as an API endpoint for integration with university management systems.

<br/>

---

<p align="center">Made with ❤️ using Python & Graph Theory</p>
