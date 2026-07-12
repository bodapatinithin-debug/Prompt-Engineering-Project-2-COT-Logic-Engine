# 🧠 Prompt Engineering Project 2: Structured Reasoning & Self-Verification

![Project](https://img.shields.io/badge/Project-DecodeLabs%20Project%202-blue)
![Prompt Engineering](https://img.shields.io/badge/Prompt-Engineering-success)
![AI Reasoning](https://img.shields.io/badge/Focus-Logical%20Reasoning-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

# 📌 Project Overview

This project demonstrates how **structured prompting** and **self-verification** improve an AI model's ability to solve logical reasoning problems.

Instead of asking for a direct answer, the prompt guides the AI to:

- Understand the problem
- Track all monetary transactions
- Verify every calculation
- Identify misleading reasoning
- Review its own solution
- Produce a logically correct final answer

The project uses the **Missing Dollar Puzzle**, a classic logical paradox that frequently confuses both humans and AI systems due to incorrect arithmetic reasoning.

---

# 🎯 Objectives

The objectives of this project are to:

- Design an effective reasoning prompt.
- Improve logical reasoning using structured instructions.
- Reduce reasoning mistakes and hallucinations.
- Compare different prompting approaches.
- Demonstrate the value of self-verification.

---

# 🧩 Problem Statement

Three friends rent a hotel room costing **€300**.

- Each friend pays **€100**.
- Later, the manager realizes the room should cost **€250**.
- He gives the bellboy **€50** to return.
- The bellboy secretly keeps **€20**.
- He returns **€10** to each friend.

Now each friend has effectively paid **€90**.

Many people incorrectly reason:

```
3 × €90 = €270

Bellboy kept €20

€270 + €20 = €290
```

### ❓ Question

**Where is the missing €10?**

---

# 💡 Why This Puzzle?

The Missing Dollar Puzzle is an excellent benchmark for logical reasoning because it requires an AI model to:

- Track multiple transactions
- Verify arithmetic
- Detect misleading calculations
- Avoid double counting
- Explain the correct accounting

---

# 📂 Repository Structure

```
Prompt-Engineering-Project-2/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── prompts/
│   ├── basic_prompt.md
│   ├── structured_prompt.md
│   └── final_prompt.md
│
├── outputs/
│   ├── basic_output.md
│   ├── structured_output.md
│   └── final_output.md
│
├── docs/
│   ├── Project_Report.md
│   ├── Evaluation.md
│   └── Reflection.md
│
└── images/
    ├── workflow.png
    ├── architecture.png
    └── comparison.png
```

---

# 📝 Prompting Approaches

## 1️⃣ Basic Prompt

```text
Solve the Missing Dollar Puzzle.
```

---

## 2️⃣ Structured Prompt

```text
Solve the puzzle.

Track every payment.

Track every refund.

Verify every calculation.

Explain every step.
```

---

## 3️⃣ Optimized Prompt

```text
You are an expert logical reasoning assistant.

Before answering:

1. Read the problem carefully.
2. Track every monetary transaction.
3. Verify every calculation.
4. Check whether the arithmetic is logically valid.
5. Review your solution.
6. Correct any mistakes if found.
7. Provide the final explanation.
```

---

# 🔍 Solution Summary

### Initial Payment

```
Friend A = €100

Friend B = €100

Friend C = €100

Total = €300
```

---

### Hotel

```
Hotel keeps €250
```

---

### Bellboy

```
Bellboy keeps €20
```

---

### Refund

```
Friends receive €30
```

---

### Verification

```
€250 + €20 + €30 = €300
```

Everything balances correctly.

There is **no missing €10**.

---

# 📊 Prompt Performance Comparison

| Feature | Basic Prompt | Structured Prompt | Optimized Prompt |
|----------|--------------|-------------------|------------------|
| Understands the Problem | ✅ | ✅ | ✅ |
| Tracks Transactions | ❌ | ✅ | ✅ |
| Verifies Calculations | ❌ | ✅ | ✅ |
| Detects Logic Trap | ❌ | ✅ | ✅ |
| Self-Verification | ❌ | ❌ | ✅ |
| Hallucination Risk | High | Medium | Low |
| Logical Accuracy | Medium | High | Very High |
| Overall Reliability | ⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |

🏆 **Best Result:** Optimized Prompt with Self-Verification

---

# 📈 Workflow

```text
Missing Dollar Puzzle
          │
          ▼
     Basic Prompt
          │
          ▼
   Direct AI Response
          │
          ▼
 Structured Prompt
          │
          ▼
 Track Transactions
          │
          ▼
 Verify Calculations
          │
          ▼
 Self-Verification
          │
          ▼
 Correct Final Answer
```

---

# 🛠 Technologies Used

- ChatGPT
- Prompt Engineering
- Markdown
- GitHub

---

# 🎓 Skills Demonstrated

- Prompt Engineering
- Structured Prompt Design
- Logical Reasoning
- Self-Verification
- Critical Thinking
- AI Evaluation
- Hallucination Reduction

---

# 📚 Learning Outcomes

After completing this project, I learned:

- How prompt design influences AI reasoning.
- The importance of structured verification.
- How logical puzzles expose reasoning weaknesses.
- How self-review improves response quality.
- How to compare different prompting strategies.

---

# 🚀 Future Improvements

- Evaluate additional reasoning puzzles.
- Compare responses across multiple AI models.
- Measure response consistency.
- Develop a benchmark dataset for logical reasoning tasks.
- Explore automated evaluation metrics.

---

# 🤝 Acknowledgements

This project was completed as part of the **DecodeLabs Prompt Engineering Internship – Project 2**.

---

# 📄 License

This project is licensed under the **MIT License**. See the `LICENSE` file for more information.
