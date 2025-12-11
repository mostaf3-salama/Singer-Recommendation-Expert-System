# 🎓 Academic Advisor Expert System

> A Rule-Based Expert System built with Python and `experta` to help students choose their college major.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue) ![Library](https://img.shields.io/badge/Library-Experta-green) ![Type](https://img.shields.io/badge/Type-Rule--Based-orange)

## 📖 Overview
This project is an Artificial Intelligence application that functions as an **Academic Advisor**. Instead of using traditional procedural programming (nested `if-else` statements), it uses a **Rule-Based Expert System** approach.

The system mimics a human counselor by:
1.  Asking the user about their interests, favorite subjects, and skills.
2.  Matching these "Facts" against a set of predefined "Rules" using an Inference Engine.
3.  Recommending the most suitable College Major.

## 🧠 How It Works (The Logic)
This system utilizes the **Rete Algorithm** (via the `experta` library) to perform pattern matching.

### The Decision Logic
The recommendations are based on the following Knowledge Base:

| User Interest | Strongest Subject | Key Skill | **Recommended Major** |
| :--- | :--- | :--- | :--- |
| Technology | Math | Logic/Problem Solving | **Computer Science** |
| Design/Art | Drawing/Physics | Creativity | **Architecture** |
| Helping People | Biology | Analysis | **Medical Field** |
| Business | Math | Leadership | **Business Administration** |

### Code Structure
* **Facts:** The inputs provided by the user (e.g., `Fact(interest='tech')`).
* **Rules:** The logic gates decorated with `@Rule`. They trigger automatically when facts match.
* **Engine:** The `KnowledgeEngine` that runs the inference cycle.

## 🛠️ Prerequisites
* Python 3.x installed.
* `experta` library.

## 🚀 Installation & Setup

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/Academic-Advisor-System.git](https://github.com/YOUR_USERNAME/Academic-Advisor-System.git)
    cd Academic-Advisor-System
    ```

2.  **Install Dependencies**
    ```bash
    pip install experta
    ```

## 💻 Usage

1.  Run the main script:
    ```bash
    python main.py
    ```

2.  Follow the on-screen prompts.
    * *Example Interaction:*
    ```text
    --- 🎓 Welcome to the AI Academic Advisor 🎓 ---
    
    Q1: What are you most interested in? [technology, design, helping_people]
    > technology
    
    Q2: What is your strongest subject? [math, biology, drawing]
    > math
    
    Q3: What is your best soft skill? [logic, creativity]
    > logic
    
    ✅ Recommendation: Computer Science (CS)
       Reason: You have a logical mind and love technology.
    ```

## 📂 Project Structure

```text
Academic-Advisor-System/
│
├── main.py            # The source code containing the Engine, Rules, and UI
├── README.md          # Project documentation (This file)
└── requirements.txt   # List of dependencies
