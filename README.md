# Travel-Planning-Multi-Agent-System
An intelligent system that coordinates multiple specialized agents to search flights, hotels, plan itineraries, and provide personalized travel recommendations.

## Step 1 - Start with the process to automate
- Search hotels and flights based on user preferences
- Plan complete travel itineraries
- Answer travel-related questions with deep research
- Handle multiple queries in parallel
- Present unified, well-formatted travel recommendation

## Step 2 & 3 - Map out your workflow as discrete steps & Identify what each steps need to do
- **Search Agent:** Handles hotel and flight search based on user preferences.
- **Itinerary Planner Agent:** Utilizes search results and research to create detailed travel plans.

## Quick Start

### 1. Install Python

**Windows (PowerShell with winget):**
```powershell
winget install Python.Python.3.X
```
Restart your terminal after installation.

**Windows (Manual installer):**
1. Download Python 3.X from https://www.python.org/downloads/
2. Run the installer
3. ✅ **Check "Add python.exe to PATH"** at the bottom of the first screen
4. Click **"Install Now"**

**Verify installation (Windows):**
```powershell
py -3.X --version
```

**macOS:**
```bash
# Using Homebrew (recommended)
brew install python@3.X

# Verify installation
python3.X --version
```

**Linux (Ubuntu/Debian):**
```bash
sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt update
sudo apt install python3.X python3.X-venv

# Verify installation
python3.X --version
```

### 2. Create a virtual environment (recommended)

**Windows (PowerShell):**
```powershell
py -3.X -m venv .venv
```

**macOS/Linux:**
```bash
python3.X -m venv .venv
```

### 4. Activate the virtual environment

**Windows (PowerShell):**
```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass; .\.venv\Scripts\Activate.ps1
```

**Windows (CMD):**
```bat
.venv\Scripts\activate.bat
```

**macOS/Linux:**
```bash
source .venv/bin/activate
```

### 5. Install dependencies
```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 6. Configure OpenAI API

**Windows (PowerShell):**
```powershell
Copy-Item .env.example .env
```

**macOS/Linux:**
```bash
cp .env.example .env
```

Then edit `.env` and set:
```env
OPENAI_API_KEY=sk-your-key-here
OPENAI_CHAT_MODEL=gpt-4o-mini
```
