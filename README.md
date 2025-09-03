# AI Agent Lab Showcase 🚀

This repository documents my learnings from the Microsoft Learn lab on building modular AI agents using Azure AI Foundry and GPT-4.1. The agent reads structured data, interprets natural language prompts, and responds with actionable insights — all deployed with future-proof architecture and clean separation of logic.

## 🧠 What This Agent Does

- Accepts structured input (e.g., category-cost breakdown)
- Responds to natural language queries like:  
  _"What's the category with the highest cost?"_
- Uses Azure-hosted GPT-4.1 model for reasoning
- Modular design for easy extension and orchestration

## 🗂️ Folder Structure

```plaintext
ai-agent-lab-showcase/
├── .env.example           # Environment config template
├── README.md              # Project overview and usage
├── requirements.txt       # Python dependencies
├── agent/
│   ├── agent.py           # Core agent logic
│   ├── utils.py           # Helper functions
│   └── prompts/
│       └── cost_analysis.txt  # Prompt templates
├── data/
│   └── data.txt           # Sample input data
├── docs/
│   └── architecture.md    # Agent flow and deployment notes
├── learnings/
│   └── reflections.md     # Personal takeaways and improvements
```
## ⚙️ Tech Stack

- **Azure AI Foundry** – Model deployment and orchestration
- **GPT-4.1 (via Azure)** – Natural language reasoning engine
- **Python 3.10+** – Agent logic and prompt handling
- **PowerShell** – Automation of file structure, Git operations, and environment setup
- **GitHub** – Version control, documentation, and public showcase

## 🧪 Setup & Run

### 1. Clone the Repository
```bash
git clone https://github.com/ksp987/ai-agent-lab-showcase.git
cd ai-agent-lab-showcase
```
### 2. Create Environment Configuration
```bash
cp .env.example .env
```
```text
Edit .env with your values:
```
```code
OPENAI_API_KEY=your-azure-openai-key
MODEL_DEPLOYMENT_NAME="gpt-4.1"
```
### 3. Install Dependencies
```text
Ensure you're using Python 3.10+ and install required packages:
```
```bash
pip install -r requirements.txt
```

### 4. Run the Agent
```text
Launch the agent from the command line:
```
```bash
python agent/agent.py
```
```text
You’ll see a prompt like:
```
```bash
Using agent: data-agent
Enter a prompt (or type 'quit' to exit):
```
### Sample Prompt
```text
Try entering:
``` 
```code
What's the category with the highest cost?
```
```text
Expected output:
```
```code
Transportation: 2301.00
```

## 📌 Key Learnings
- Diagnosed and resolved invalid_engine_error by aligning model deployment names
- Structured agent logic for modularity and reusability
- Used PowerShell to automate repo setup and Git operations
- Documented architecture and reflections for future scalability
- Practiced clean Git hygiene and repo isolation for public showcase

## 🧭 Next Steps
- Add GitHub Actions for automated validation and deployment
- Publish architecture diagrams and technical reflections

