
# Data Analysis + LLM Curriculum (Python, R, **PydanticAI** with Ollama)

A 12-week, project-based roadmap for learning **data analysis**, **Unix/Linux basics**, and **LLM apps** using **Python**, **R**, **PydanticAI**, and **Ollama** (local models).  
All resources are **100% free** and include lectures, interactive projects, GitHub practice, and an **optional "cool kids" track** with Neovim + CLI tools.

---

## Week -1: Mac + Homebrew Setup Checklist

### Step 1: Install Python + Tools
- [ ] Install Python 3.11 → `brew install python@3.11`
- [ ] Install uv package manager → `brew install uv`
- [ ] Install Git → `brew install git`
- [ ] Install iTerm2 → `brew install --cask iterm2`
- [ ] Install VSCode → `brew install --cask visual-studio-code`
- [ ] Verify Python version → `python3 --version`

### Step 2: Install R + RStudio
- [ ] Install R → `brew install --cask r`
- [ ] Install RStudio → `brew install --cask rstudio`

### Step 3: Install JupyterLab
- [ ] Install JupyterLab → `uv pip install jupyterlab`
- [ ] Run Jupyter → `jupyter lab`

### Step 4: Install Data Science Libraries
- [ ] Install NumPy → `uv pip install numpy`
- [ ] Install pandas → `uv pip install pandas`
- [ ] Install matplotlib → `uv pip install matplotlib`
- [ ] Install seaborn → `uv pip install seaborn`
- [ ] Install SciPy → `uv pip install scipy`
- [ ] Install statsmodels → `uv pip install statsmodels`

### Step 5: Install AI Stack
- [ ] Install Pydantic → `uv pip install pydantic`
- [ ] Install PydanticAI → `uv pip install pydantic-ai`
- [ ] Install ChromaDB → `uv pip install chromadb`

### Step 6: Install Ollama
- [ ] Install Ollama → `brew install ollama`
- [ ] Pull Llama3.1 model → `ollama pull llama3.1`
- [ ] Pull nomic-embed-text model → `ollama pull nomic-embed-text`
- [ ] Test Ollama → `ollama run llama3.1 "Hello world"`

### Step 7: Create Project Folder
- [ ] Create project folder → `mkdir data-analyst-curriculum && cd data-analyst-curriculum`
- [ ] Create virtual environment → `uv venv .venv`
- [ ] Activate environment → `source .venv/bin/activate`

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

