# Coder

Agentic **code assistant** that autonomously plans, writes, and evaluates code using multi‑agent collaboration.

- Built with **CrewAI** for orchestrating coding agents.

## Project Structure
```
coder_clean/
├─ knowledge/
│  └─ user_preference.txt
├─ output/
│  ├─ .gitkeep
│  └─ code_and_output.txt
├─ src/
│  └─ coder/
│     ├─ config/
│     │  ├─ agents.yaml
│     │  └─ tasks.yaml
│     ├─ tools/
│     │  ├─ __init__.py
│     │  └─ custom_tool.py
│     ├─ __init__.py
│     ├─ crew.py
│     └─ main.py
├─ .gitignore
├─ pyproject.toml
├─ README.md
└─ uv.lock
```
## Quick Start
### 1) Prerequisites
- Python **>= 3.10, < 3.13**
- `.env` file containing your API key(s):
```
OPENAI_API_KEY=sk-...
```

### 2) Install
```bash
pip install uv
uv pip install -e .
```

### 3) Configure
- Update agents and tasks under `config/`.
- Generated code and logs stored in `output/`.

### 4) Run
```bash
python -m src.coder.main
```

## GitHub: Publish
```bash
git init
git add .
git commit -m "Initial commit: Coder agents"
git branch -M main
git remote add origin https://github.com/<YOUR_USERNAME>/coder.git
git push -u origin main
```

## Notes
- Cleaned environment and build artifacts removed.
- `output/` kept empty in Git using `.gitkeep`.
