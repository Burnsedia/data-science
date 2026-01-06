# Setup Guide

This guide walks you through setting up your development environment for the Data Analysis + LLM Curriculum. The curriculum supports Mac, Ubuntu/WSL, and Arch Linux. We prioritize UV for fast Python package management and include modern tools like PyTorch and Ruff.

## Prerequisites

- A computer with internet access.
- Basic command-line familiarity (covered in Week 0).
- For WSL: Windows 10/11 with virtualization enabled.

## Why These Tools?

- **Python 3.12**: Latest stable version with performance improvements and new features.
- **UV**: Ultra-fast Python package installer (faster than pip).
- **Ollama**: Local LLM runner for privacy and offline AI work.
- **JupyterLab**: Interactive notebooks for data exploration.
- **VS Code**: Versatile editor with Python/R support.
- **R & RStudio**: For statistical computing and visualization.
- **Modern Libraries**: PyTorch for ML, Plotly for interactive charts, Ruff for linting.

## Universal Steps (All Platforms)

1. **Install Git**: Version control for projects.
   - Download from https://git-scm.com/ or use platform commands below.

2. **Install UV**: `pip install uv` (ensure pip is available via Python).

3. **Install VS Code**: Download from https://code.visualstudio.com/. Install extensions: Python, R, Jupyter.

4. **Install Ollama**: Download from https://ollama.ai/. Follow the installer for your OS.
   - Pull models: `ollama pull llama3.1` and `ollama pull nomic-embed-text`.
   - Test: `ollama run llama3.1 "Hello world"`.

5. **Create Project Folder**:
   ```
   mkdir data-analyst-curriculum
   cd data-analyst-curriculum
   uv venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

## Platform-Specific Instructions

### Mac (using Homebrew)

1. Install Homebrew: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
2. Install Python: `brew install python@3.12`
3. Install Git: `brew install git`
4. Install iTerm2: `brew install --cask iterm2` (better terminal).
5. Install R: `brew install --cask r`
6. Install RStudio: `brew install --cask rstudio`
7. Verify: `python3 --version` (should be 3.12.x)

### Ubuntu/WSL (using apt)

1. Update system: `sudo apt update && sudo apt upgrade -y`
2. Install Python: `sudo apt install python3.12 python3.12-venv`
3. Install Git: `sudo apt install git`
4. Install R: `sudo apt install r-base`
5. Install RStudio: Download .deb from https://posit.co/download/rstudio-desktop/ and `sudo dpkg -i rstudio-*.deb; sudo apt install -f`
6. (WSL only) Enable: On Windows, run `wsl --install -d Ubuntu`
7. Verify: `python3 --version`

### Arch Linux (using pacman)

1. Install Python: `pacman -S python`
2. Install Git: `pacman -S git`
3. Install R: `pacman -S r`
4. Install RStudio: `pacman -S rstudio-desktop` (or `yay -S rstudio-desktop` from AUR)
5. Verify: `python --version`

## Install Data Science Libraries

Activate your venv: `source .venv/bin/activate`

- JupyterLab: `uv install jupyterlab` → Run with `jupyter lab`
- Core libs: `uv install numpy pandas matplotlib seaborn scipy statsmodels`
- Modern ML: `uv install torch torchvision torchaudio` (PyTorch)
- Interactive Viz: `uv install plotly`
- Linting: `uv install ruff` → Use `ruff check .` to lint code

## Install AI Stack

- Pydantic: `uv install pydantic`
- PydanticAI: `uv install pydantic-ai`
- ChromaDB: `uv install chromadb`

## Troubleshooting

- **Python not found**: Ensure PATH includes Python (e.g., on Mac: `echo 'export PATH="/usr/local/opt/python@3.12/bin:$PATH"' >> ~/.zshrc`)
- **UV issues**: Install via pip first: `python3 -m pip install uv`
- **Ollama models slow**: Use smaller models like `llama3.1:8b` if needed.
- **WSL networking**: Ensure WSL has internet; restart with `wsl --shutdown && wsl`
- **Arch AUR**: Use `yay` or `paru` for AUR packages.

## Next Steps

Once setup is complete, proceed to [Week 0](week0.md).