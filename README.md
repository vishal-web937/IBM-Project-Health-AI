# 📘 Health AI Assistant

## 📖 Overview
The **Health AI Assistant** is a machine learning–powered tool built with **Hugging Face Transformers**, **PyTorch**, and **Gradio**.

It provides two main functionalities:
1. **Disease Prediction** – Generates possible medical conditions and general recommendations based on user-provided symptoms.
2. **Treatment Plans** – Suggests general treatment plans (including home remedies and medication guidelines) tailored to patient details.

⚠️ **Disclaimer:** This tool is **for informational purposes only**. It should **never replace professional medical advice**. Always consult a healthcare provider for diagnosis and treatment.

---

## ⚙️ Installation & Requirements
```bash
pip install transformers torch gradio
```

---

## 🏗️ How It Works
- Uses the pretrained language model **ibm-granite/granite-3.2-2b-instruct**.
- Wraps the model in a **Gradio interface** for easy interaction.
- Accepts user inputs:
  - **Symptoms** → Outputs possible conditions and general advice.
  - **Condition + Patient Info** → Outputs a personalized treatment plan.

---

## 🔧 Functions

### 1. `generate_response(prompt, max_length=1024)`
- Sends a text prompt to the model and retrieves a response.

### 2. `disease_prediction(symptoms)`
- Predicts possible conditions and recommendations based on symptoms.

### 3. `treatment_plan(condition, age, gender, medical_history)`
- Suggests a personalized treatment plan.

---

## 🖥️ Usage Guide

### Run the App
```bash
python health_ai.py
```

### Interface
The Gradio interface provides **two tabs**:

1. **Disease Prediction**
   - Enter symptoms (e.g., "fever, cough, headache").
   - Click **Analyze Symptoms**.

2. **Treatment Plans**
   - Enter condition, age, gender, and medical history.
   - Click **Generate Treatment Plan**.

---

## ⚠️ Important Notes
- This tool **does not provide medical diagnoses**.
- Always verify results with a **licensed healthcare professional**.
- Use responsibly for **educational or supportive purposes** only.
