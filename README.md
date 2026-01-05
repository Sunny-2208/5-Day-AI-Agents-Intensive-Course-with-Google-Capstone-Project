# 5-Day-AI-Agents-Intensive-Course-with-Google-Capstone-Project
SmartClaimX is a multi-agent AI system that automates health insurance claim validation. It coordinates specialized agents for policy coverage, fraud detection, medical validity, and cost estimation to produce structured, explainable claim decisions using Google Gemini and ADK workflows.

<img width="1562" height="784" alt="image" src="https://github.com/user-attachments/assets/d35fee13-cd0e-4592-b77d-80aa4c41c35f" />

---

### 🔹 Features
- **End-to-End Claim Analysis:** Takes raw claim text and outputs a structured decision:  
  ✔ Approve | ❌ Reject | ⚠ Review / Investigate  
- **Explainable Decisions:** Per-agent outputs clarify why each claim was evaluated that way.  
- **Fully Automated & Modular:** Easy to extend to real insurance datasets.  

---

### 🔹 Multi-Agent Architecture (A2A – Agent-to-Agent Workflow)
SmartClaimX uses specialized agents for specific tasks:

| Agent | Role |
|-------|------|
| `PolicyCheckerAgent` | Checks policy rules and coverage |
| `FraudDetectorAgent` | Detects suspicious patterns |
| `MedicalValidationAgent` | Validates medical correctness using ICD mappings |
| `CostEstimatorAgent` | Extracts claimed amount & verifies reasonability |
| `CoordinatorAgent` | Orchestrates all agents & produces final decision |

**Workflow:** Parallel reasoning with sequential pipeline orchestration ensures efficiency and accuracy.  

---

### 🔹 Core Concepts & Tools
- **Parallel Agents:** Concurrent reasoning for faster analysis  
- **Sequential Agent Pipeline:** Structured task execution  
- **FunctionTool:** Python function execution for agent tasks  
- **InMemoryRunner:** Local simulation of workflows  
- **Observability:** Session memory & logging for transparency  
- **GUI Interface:** Interactive control via `ipywidgets`  

---

### 🔹 Technology Stack
- **Agent Platform:** Google Agent Development Kit (ADK)  
- **AI Models:** Gemini 2.0  
- **Programming Language:** Python  
- **Interface:** Jupyter notebook / ipywidgets  

---

### 🔹 How It Works
1. Input raw claim text  
2. Coordinator dispatches tasks to specialized agents  
3. Agents process the claim concurrently and sequentially as needed  
4. Outputs are combined into a final decision with detailed reasoning


## 🚀 How to Run on Kaggle  

### 1. Open the Notebook
- Open this project in **Kaggle Notebook** (either fork or upload).  

---

### 2. Add Google API Key in Kaggle Secrets
1. In Kaggle, go to **Add-ons → Secrets**.  
2. Click **New Secret**.  
3. Enter:  
   - **Secret Name:** `GOOGLE_API_KEY`  
   - **Secret Value:** (Paste your API Key from [Google AI Studio](https://aistudio.google.com/app/apikey))  
4. Save it.  

---

### 3. Run the Notebook 
- Click on Run All 
- Paste sample report pdf or paste the report in text box
- Click Analyze Report

---
