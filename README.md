
# 🧠 Code Agent + Data Analyzer (Flowise AI)

This project is a **Code Execution & Data Analysis Agent** built in [Flowise AI](https://flowiseai.com/), powered by **Groq LLM**, **E2B Code Interpreter**, and **Memory Integration**. It can understand user queries, write Python code, execute it in a sandbox, and return results — making it ideal for **data analysis, visualization, and automation**.

---
<img width="1366" height="616" alt="Image" src="https://github.com/user-attachments/assets/ee99f757-da31-4b06-b29b-83d62d01639a" />
<img width="1366" height="609" alt="Image" src="https://github.com/user-attachments/assets/7ffa4f17-43ee-4aa3-a298-90ea6b6b61e8" />
<img width="1366" height="628" alt="Image" src="https://github.com/user-attachments/assets/f6bb25e1-a2b3-4553-b9d1-0b3698688fdd" />
<img width="1366" height="572" alt="Image" src="https://github.com/user-attachments/assets/d2254b3e-62a8-4ad4-bf80-0a7f1d72925f" />

## 📌 Features

- **Groq LLM Integration** – Uses `deepseek-r1-distill-llama-70b` for fast, high-quality reasoning.
- **E2B Code Interpreter** – Executes Python code in a secure sandbox with libraries like `numpy`, `pandas`, `matplotlib`, and more.
- **Data Analysis Capabilities** – Handles CSV/Excel processing, visualization, statistical analysis, and ML workflows.
- **Memory Support** – Maintains chat context for multi-step problem solving.
- **Agent Execution** – Uses **Tool Agent** with function calling to decide when to run code vs. when to answer directly.

---

## 🛠 Tech Stack

- **Flowise AI**
- **Groq API** (LLM backend)
- **E2B API** (Code execution)
- **Python Data Libraries** (`pandas`, `numpy`, `matplotlib`, `scipy`, etc.)
- **LangChain** Agent Executor
- **Buffer Memory** for context retention

---

## 🚀 Getting Started

### 1️⃣ Prerequisites

Before running this project, you’ll need:
- **Node.js** v18+
- **Flowise AI** installed
- **Groq API Key** ([Get it here](https://groq.com/))
- **E2B API Key** ([Get it here](https://e2b.dev/))

---

### 2️⃣ Installation

```bash
# Clone repository
git clone https://github.com/yourusername/code-agent-data-analyzer.git
cd code-agent-data-analyzer

# Install Flowise globally if not already installed
npm install -g flowise

# Start Flowise
npx flowise start
```

---

### 3️⃣ Import Chatflow

1. Open [http://localhost:3000](http://localhost:3000) after starting Flowise.
2. Click **Import Chatflow**.
3. Upload the `Data Analyzer Chatflow.json` file from this repo.
4. Update API keys for **Groq** and **E2B** in the Flowise credentials section.

---

### 4️⃣ Environment Variables

In Flowise or `.env`:
```
GROQ_API_KEY=your_groq_api_key
E2B_API_KEY=your_e2b_api_key
```

---

## 📂 Project Structure

```
.
├── Data Analyzer Chatflow.json  # Flowise chatflow configuration
├── README.md                    # Project documentation
```

---

## 🧩 How It Works

1. **GroqChat Node** – Receives user instructions, powered by Groq LLM.
2. **Tool Agent Node** – Decides whether to use code execution.
3. **Code Interpreter (E2B)** – Runs Python code, processes data, and generates visualizations.
4. **Buffer Memory Node** – Retains conversation history for multi-step reasoning.

---

## 🖥 Usage

- Start Flowise and open the chat UI.
- Ask natural language questions like:
  - *"Load this CSV and calculate the average sales per month."*
  - *"Generate a scatter plot of population vs GDP from this dataset."*
  - *"Train a linear regression model on this dataset."*
- The agent will generate Python code, execute it, and return results.

---

## 🔮 Future Enhancements

- Support for **R** and **JavaScript** code execution.
- Integration with **SQL databases**.
- Enhanced **data visualization templates**.

---

## 📜 License

This project is licensed under the **MIT License**.
