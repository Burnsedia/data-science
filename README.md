# Data Analysis + LLM Curriculum (Python, R, **PydanticAI** with Ollama)

A 12-week, project-based roadmap for learning **data analysis**, **Unix/Linux basics**, and **LLM apps** using **Python**, **R**, **PydanticAI**, and **Ollama** (local models).  
Now updated for **cross-platform support** (Mac, Ubuntu/WSL, Arch Linux) with modern tools like PyTorch, Plotly, and Ruff.  
All resources are **100% free** and include lectures, interactive projects, GitHub practice, and an **optional "cool kids" track** with Neovim + CLI tools.

---

## Week -1: Cross-Platform Setup Checklist

This curriculum supports Mac, Ubuntu/WSL, and Arch Linux. Choose your platform below. UV is the preferred Python package manager for its speed. Python 3.12 is recommended for modern features.

### Universal Steps (All Platforms)
- [ ] Install Git (see platform-specific below)
- [ ] Install UV → `pip install uv` (or via platform package manager if available)
- [ ] Install VS Code (download from https://code.visualstudio.com/)
- [ ] Install Ollama (download from https://ollama.ai/ and follow platform installer)
- [ ] Pull Llama3.1 model → `ollama pull llama3.1`
- [ ] Pull nomic-embed-text model → `ollama pull nomic-embed-text`
- [ ] Test Ollama → `ollama run llama3.1 "Hello world"`
- [ ] Create project folder → `mkdir data-analyst-curriculum && cd data-analyst-curriculum`
- [ ] Create virtual environment → `uv venv .venv`
- [ ] Activate environment → `source .venv/bin/activate`

### Platform-Specific Steps

#### Mac (using Homebrew)
- [ ] Install Homebrew → `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
- [ ] Install Python 3.12 → `brew install python@3.12`
- [ ] Install Git → `brew install git`
- [ ] Install iTerm2 → `brew install --cask iterm2`
- [ ] Install R → `brew install --cask r`
- [ ] Install RStudio → `brew install --cask rstudio`
- [ ] Verify Python version → `python3 --version`

#### Ubuntu/WSL (using apt)
- [ ] Update system → `sudo apt update && sudo apt upgrade -y`
- [ ] Install Python 3.12 → `sudo apt install python3.12 python3.12-venv`
- [ ] Install Git → `sudo apt install git`
- [ ] Install R → `sudo apt install r-base`
- [ ] Install RStudio → Download .deb from https://posit.co/download/rstudio-desktop/ and `sudo dpkg -i rstudio-*.deb`
- [ ] Verify Python version → `python3 --version`
- [ ] (WSL only) Enable WSL if not done: On Windows, run `wsl --install -d Ubuntu`

#### Arch Linux (using pacman - Flex Mode)
- [ ] Install Python → `pacman -S python`
- [ ] Install Git → `pacman -S git`
- [ ] Install R → `pacman -S r`
- [ ] Install RStudio → `pacman -S rstudio-desktop` (or from AUR: `yay -S rstudio-desktop`)
- [ ] Verify Python version → `python --version`

### Step 3: Install Data Science Libraries (All Platforms)
- [ ] Install JupyterLab → `uv install jupyterlab`
- [ ] Run Jupyter → `jupyter lab`
- [ ] Install NumPy → `uv install numpy`
- [ ] Install pandas → `uv install pandas`
- [ ] Install matplotlib → `uv install matplotlib`
- [ ] Install seaborn → `uv install seaborn`
- [ ] Install SciPy → `uv install scipy`
- [ ] Install statsmodels → `uv install statsmodels`
- [ ] Install PyTorch (for modern ML) → `uv install torch torchvision torchaudio`
- [ ] Install Plotly (for interactive viz) → `uv install plotly`
- [ ] Install Ruff (modern linter) → `uv install ruff`

### Step 4: Install AI Stack (All Platforms)
- [ ] Install Pydantic → `uv install pydantic`
- [ ] Install PydanticAI → `uv install pydantic-ai`
- [ ] Install ChromaDB → `uv install chromadb`

---

## Suggested Repo Layout

```text
data-analyst-curriculum
├── 01_unix_linux
├── 02_python_basics
├── 03_pandas_eda
├── 04_stats_intro
├── 05_r_tidyverse
├── 06_pydanticai_rag
├── 07_pydanticai_assistant
├── 08_sql_tooling
├── 09_eval_observability
└── capstones
    ├── analyst_copilot_pydanticai
    └── r_eda_report
```
```
````
---

## Week 0: CS & Unix/Linux
### Lectures
- [ ] [CS50’s Introduction to Computer Science (Harvard)](https://cs50.harvard.edu/x/)  
- [ ] [freeCodeCamp – Linux for Beginners (4 hrs)](https://www.youtube.com/watch?v=sWbUDq4S6Y8)  
- [ ] [MIT Missing Semester – Shell Tools & Scripting](https://missing.csail.mit.edu/2020/shell-tools/)  

### Interactive
- [ ] [OverTheWire – Bandit Wargame](https://overthewire.org/wargames/bandit/) *(hands-on Linux terminal practice)*  

---

## Weeks 1–3: Python Foundations + Unix/Linux Basics
### Lectures
- [ ] [freeCodeCamp – Python for Beginners (4 hrs)](https://www.youtube.com/watch?v=eWRfhZUzrAc)
- [ ] [Kaggle – Python Course](https://www.kaggle.com/learn/python)  
- [ ] [CS50’s Introduction to Python (Harvard)](https://cs50.harvard.edu/python/2022/)  

### Interactive Projects
- [ ] [freeCodeCamp – Scientific Computing with Python Certification](https://www.freecodecamp.org/learn/scientific-computing-with-python/)  
   *Projects:* Arithmetic Formatter, Time Calculator, Budget App, Polygon Area Calculator, Probability Calculator  

---

## Weeks 4–5: Statistics & R
### Lectures
- [ ] [Khan Academy – Statistics & Probability](https://www.khanacademy.org/math/statistics-probability)  
- [ ] [StatQuest with Josh Starmer](https://www.youtube.com/user/joshstarmer)  
- [ ] [MIT OCW – Probability & Statistics](https://ocw.mit.edu/courses/res-6-012-introduction-to-probability-spring-2018/)  
- [ ] [freeCodeCamp – R Programming for Data Science (2 hrs)](https://www.youtube.com/watch?v=_V8eKsto3Ug)  
- [ ] [R for Data Science (Book)](https://r4ds.had.co.nz/)  

### Interactive Projects
- [ ] [freeCodeCamp – Data Analysis with Python Certification](https://www.freecodecamp.org/learn/data-analysis-with-python/)  
   *Projects:* Mean-Variance Calculator, Demographic Data Analyzer, Medical Data Visualizer, Time Series Visualizer, Sea Level Predictor  

---

## Weeks 6–7: Python for Data Analysis
### Lectures
- [ ] [freeCodeCamp – Data Analysis with Python (5 hrs)](https://www.youtube.com/watch?v=r-uOLxNrNk8)  
- [ ] [Kaggle – Pandas Course](https://www.kaggle.com/learn/pandas)  
- [ ] [Kaggle – Data Visualization Course](https://www.kaggle.com/learn/data-visualization)  

### Interactive
- [ ] Finish [freeCodeCamp Data Analysis with Python Certification](https://www.freecodecamp.org/learn/data-analysis-with-python/)  

---

## Weeks 6–12: LLMs, PydanticAI & AI Agents
### Lectures
- [ ] [freeCodeCamp – LangChain for Beginners](https://www.youtube.com/watch?v=lG7Uxts9SXs) *(concepts apply to PydanticAI)*  
- [ ] [DeepLearning.AI – Free Short Courses on LLMs](https://learn.deeplearning.ai/)  

---

## Week 10: SQL & Databases
### Lectures
- [ ] [freeCodeCamp – SQL Full Course (4 hrs)](https://www.youtube.com/watch?v=HXV3zeQKqGY)  
- [ ] [Khan Academy – Intro to SQL](https://www.khanacademy.org/computing/computer-programming/sql)  

### Interactive Projects
- [ ] [freeCodeCamp – Relational Database Certification](https://www.freecodecamp.org/learn/relational-database/)  
   *Projects:* Celestial Bodies Database, World Cup Database, Salon Scheduler, Number Guessing Game  

---

## Weeks 11–12: Capstones & Projects
### Resources
- [ ] [Kaggle – Free Datasets](https://www.kaggle.com/datasets)  
- [ ] [DataCamp Workspace (Free Tier)](https://www.datacamp.com/workspace)  
- [ ] [MIT OCW – Data Science & Machine Learning](https://ocw.mit.edu/search/?t=data+science)  

### Interactive Projects
- [ ] [freeCodeCamp – Machine Learning with Python Certification](https://www.freecodecamp.org/learn/machine-learning-with-python/)  
   *Projects:* Rock, Paper, Scissors AI, Cat/Dog Classifier, Book Recommender, Stock Predictor, Neural Network SMS Classifier  

---

## Git & GitHub (Do This Throughout)
- [ ] [GitHub – Hello World Guide](https://docs.github.com/en/get-started/start-your-journey/hello-world)  
- [ ] [freeCodeCamp – Git & GitHub for Beginners (2 hrs)](https://www.youtube.com/watch?v=RGOj5yH7evk)  
- [ ] [Oh My Git! – Interactive Git Game](https://ohmygit.org/)  

### Weekly GitHub Habits
- [ ] Create a repo for each week/project  
- [ ] Add `README.md` summarizing what was learned  
- [ ] Commit often (`git add . && git commit -m "message" && git push`)  
- [ ] Upload Jupyter Notebooks (render well on GitHub)  
- [ ] Pin best repos to showcase skills  

---

## ⚡ Optional: "Cool Kids" Neovim + CLI Tools Track

### Neovim Setup
- [ ] Install Neovim → `brew install neovim`
- [ ] Learn basics: `i` (insert), `:wq` (save & quit), `dd` (delete line), `/` (search)
- [ ] [freeCodeCamp – Vim Tutorial for Beginners (2 hrs)](https://www.youtube.com/watch?v=RZ4p-saaQkc)  
- [ ] Explore config: `~/.config/nvim/init.lua`  

### CLI Tools (Make Linux fun & powerful)
- [ ] Install **fzf** (fuzzy finder) → `brew install fzf`
- [ ] Install **ripgrep** (fast search) → `brew install ripgrep`
- [ ] Install **htop** (system monitor) → `brew install htop`
- [ ] Install **bat** (better `cat`) → `brew install bat`
- [ ] Install **exa** (better `ls`) → `brew install exa`
- [ ] Bonus: Try **tmux** for terminal multiplexing → `brew install tmux`

### Practice
- [ ] Replace basic commands: `cat → bat`, `ls → exa`
- [ ] Use `fzf` to search command history
- [ ] Use `ripgrep` to search code fast
- [ ] Manage processes with `htop`
- [ ] Keep multiple projects open in `tmux`  

---

✅ Finish Week -1 through Week 12, sprinkle in the optional “cool kids” track, and she’ll have a full **data + AI + Linux toolkit** with a strong GitHub portfolio.



## 📊 Data Analysis + LLM Projects (Week-by-Week)

This project roadmap matches the 12-week curriculum. All projects are aligned to tools introduced that week, and many include LLM integration using **PydanticAI** and **Ollama**.

---

### ✅ Week 0: CS & Unix/Linux

**Project:** Command Line File Audit Tool

* Write a Python CLI tool to summarize number, type, and size of files in a directory.
* Optional: Output as a CSV report.

---

### ✅ Week 1: Python Fundamentals

**Project:** Python Expense Tracker (CLI)

* Build a simple CLI that logs expenses and categorizes them.
* Output to CSV with `pandas`.
* Stretch: Add terminal charts with `rich` or `plotext`.

---

### ✅ Week 2: Python Functions + CLI Skills

**Project:** CSV Column Analyzer

* Let users input a CSV and return column types, null counts, and stats.
* Use `pydantic-ai` to summarize or rephrase the report via LLM.

---

### ✅ Week 3: Basic EDA in Python

**Project:** Netflix Dataset EDA

* Use `pandas`, `matplotlib`, and `seaborn` to explore the [Netflix dataset](https://www.kaggle.com/shivamb/netflix-shows).
* Ask Ollama to suggest plots or describe patterns with `pydantic-ai` schema outputs.

---

### ✅ Week 4: Statistics with Python

**Project:** Survey Summary Generator

* Take a small dataset of survey results.
* Use Python to calculate means, modes, distributions.
* Ask LLM to generate a Markdown report with PydanticAI.

---

### ✅ Week 5: Intro to R & Tidyverse

**Project:** R Data Explorer

* Use R (`dplyr`, `ggplot2`) to generate a basic report of any dataset.
* Export tables/plots.
* Bonus: Knit an `.Rmd` to HTML.

---

### ✅ Week 6: Advanced Pandas

**Project:** Airbnb Dataset EDA Bot

* Use Kaggle's NYC Airbnb dataset.
* Build a CLI or notebook that allows user to:

  * Load data
  * Ask questions
  * Get answers powered by Ollama + PydanticAI

---

### ✅ Week 7: Data Cleaning with LLMs

**Project:** Dirty CSV Fixer

* Input: Messy CSV (with typos, missing units, bad formats).
* Define a schema with `pydantic-ai`.
* LLM suggests cleaned rows and explanations.

---

### ✅ Week 8: CSV Q\&A Assistant

**Project:** CSV Chat Agent

* Upload a CSV and ask natural questions ("What’s the avg revenue in Q1?").
* Use `pydantic-ai` + `chromadb` + `ollama` for retrieval.

---

### ✅ Week 9: PDF Report Analyzer

**Project:** PDF → Markdown Extractor

* Load a multi-page PDF report (e.g. economic data).
* Use PyMuPDF to extract text.
* Ask LLM to generate a summary and key metrics as Markdown.

---

### ✅ Week 10: SQL + LLM

**Project:** Natural Language to SQL

* Load a SQLite database (e.g. ecommerce).
* User types: "Top 5 customers by revenue."
* LLM generates SQL → fetch results → show as table or chart.

---

### ✅ Week 11: Capstone Prep

**Project:** Analyst Copilot (Part 1)

* Combine multiple tools:

  * Ask a question
  * Pull from CSV + SQL
  * Output: Graphs + Summary + raw data
* Use `pydantic-ai` to structure answers.

---

### ✅ Week 12: Capstone Final

**Project:** Analyst Copilot (Final)

* Wrap up with a CLI or Web UI (Streamlit).
* Multi-modal assistant: PDF + CSV + SQL.
* Structured answers + human-friendly output.
* Host on GitHub with full documentation.

---

These projects ensure hands-on practice across **data analysis**, **LLM-powered workflows**, and reproducible portfolio-building with Python, R, SQL, and PydanticAI.

