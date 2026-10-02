# Team Combinatorial Optimization Using Local Search Metaheuristics

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Google Colab](https://img.shields.io/badge/Environment-Google%20Colab-orange.svg)](https://colab.research.google.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📌 Overview

This repository contains an Artificial Intelligence research project developed for the **Bachelor of Information Systems (BSI)** degree. 

The main goal is to solve a **Combinatorial Team Optimization Problem** within the turn-based strategy browser game *Naruto-Arena Classic*. The system models character abilities, chakra synergy, damage outputs, and crowd control mechanics into a custom **Objective Function**, evaluated through two local search metaheuristics: **Hill-Climbing** and **Simulated Annealing**.

---

## 🎯 Objectives

1. **Automated Data Scraping:** Extract updated character stats, skill descriptions, chakra costs, and cooldowns using Selenium in Headless mode.
2. **Feature Engineering & Parsing:** Translate raw natural language skill descriptions into structured numerical metrics.
3. **Objective Function Formulation:** Evaluate a 3-character team composition based on chakra efficiency, damage output, and utility balance.
4. **Metaheuristic Comparison:** Compare convergence speed and solution quality between **Hill-Climbing** (Steepest-Ascent / Stochastic) and **Simulated Annealing**.

---

## 🏗️ Project Architecture

```text
team-combinatorial-optimization-ai/
├── .gitignore                   # Ignored build and temporary files
├── README.md                    # Project documentation
├── requirements.txt             # Project dependencies
│
├── data/
│   ├── raw/                     # Extracted raw JSON files from scraper
│   └── processed/               # Parsed and structured dataset
│
├── notebooks/
│   ├── 01_data_scraping.ipynb   # Selenium headless web scraper
│   ├── 02_data_parsing.ipynb    # Text processing and feature extraction
│   └── 03_team_optimization.ipynb # Hill-Climbing vs. Simulated Annealing
│
└── src/
    ├── __init__.py
    ├── scraper.py               # Web scraping module
    ├── parser.py                # Skill description parser
    ├── evaluator.py             # Objective function implementation
    └── algorithms.py            # Hill-Climbing & Simulated Annealing
```

🛠️ Tech Stack
Language: Python 3.10+

Environment: Google Colab

Data Scraping & Parsing: Selenium, BeautifulSoup4, Regex

Data Manipulation & Analysis: Pandas, NumPy

Optimization Heuristics: Custom implementations of Hill-Climbing and Simulated Annealing

Visualization: Matplotlib, Seaborn

Version Control: Git & GitHub

🚀 How to Run (Google Colab)
Open Google Colab and clone this repository:

Python
!git clone [https://github.com/felixp90/team-combinatorial-optimization-ai.git](https://github.com/felixp90/team-combinatorial-optimization-ai.git)
Navigate to the notebooks folder:

Python
%cd team-combinatorial-optimization-ai/notebooks
Run 01_data_scraping.ipynb to execute the Selenium scraper and generate the raw dataset.

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
