# Project Report

# Prompt Engineering Project 2
## Chain-of-Thought (CoT) Logic Engine

**Name:** Bodapati Nithin  
**Organization:** DecodeLabs  
**Batch:** 2026

---

# 1. Introduction

Large Language Models (LLMs) are capable of solving many problems, but they sometimes generate incorrect answers due to incomplete reasoning or logical errors. Prompt Engineering helps improve AI responses by providing structured instructions that guide the reasoning process.

This project demonstrates how Chain-of-Thought (CoT) prompting improves logical reasoning using the **Missing Dollar Puzzle**, a classic logical paradox that often confuses both humans and AI systems.

---

# 2. Objective

The main objective of this project is to design a prompt that encourages an AI model to solve a logical puzzle through structured reasoning rather than guessing.

The project aims to:

- Improve logical reasoning.
- Reduce hallucinations.
- Force the AI to verify calculations.
- Compare normal prompting with structured prompting.
- Demonstrate self-verification.

---

# 3. Problem Statement

Three friends rent a hotel room costing **€300**.

Each friend pays **€100**.

Later, the hotel manager realizes the room should have cost only **€250**.

The manager gives the bellboy **€50** to return.

The bellboy secretly keeps **€20** and returns **€10** to each friend.

Now each friend has effectively paid **€90**.

Many people incorrectly reason as follows:

```
3 × €90 = €270

Bellboy kept €20

€270 + €20 = €290
```

The question is:

**Where is the missing €10?**

---

# 4. Why This Puzzle?

The Missing Dollar Puzzle was selected because it contains a misleading arithmetic calculation that often leads to incorrect conclusions.

This puzzle is suitable for evaluating AI reasoning because it requires the model to:

- Understand the story.
- Track every transaction.
- Verify calculations.
- Detect incorrect arithmetic.
- Avoid hallucinations.
- Perform self-correction.

---

# 5. Prompt Design

Three prompting strategies were used.

## Basic Prompt

```
Solve the Missing Dollar Puzzle.
```

---

## Structured Prompt

```
Solve the puzzle.

Track every payment.

Track every refund.

Verify every calculation.

Explain every step.
```

---

## Optimized Chain-of-Thought Prompt

```
You are an expert logical reasoning assistant.

Instructions:

1. Read the problem carefully.
2. Track every payment.
3. Track every refund.
4. Verify all calculations.
5. Detect incorrect assumptions.
6. Review your reasoning.
7. Correct mistakes if found.
8. Provide the final explanation.
```

---

# 6. Solution Process

The AI followed these steps:

1. Calculated the total payment.
2. Calculated the correct hotel charge.
3. Tracked the refund.
4. Identified the bellboy's share.
5. Verified the total amount.
6. Reviewed every calculation.
7. Produced the final explanation.

---

# 7. Self-Verification

The AI checked whether:

- Initial payment equals €300.
- Hotel received €250.
- Bellboy kept €20.
- Friends received €30 back.

Verification:

```
250 + 20 + 30 = 300
```

The calculations are correct.

No money is missing.

---

# 8. Results

The optimized prompt produced a significantly better explanation than the basic prompt.

Instead of directly answering the puzzle, the AI verified each transaction and identified that the mistake comes from adding the bellboy's €20 to the €270, even though the €20 is already included in the €270.

---

# 9. Comparison

| Feature | Basic Prompt | Structured Prompt | CoT Prompt |
|----------|--------------|-------------------|------------|
| Step-by-step reasoning | ❌ | ✅ | ✅ |
| Logical verification | ❌ | ✅ | ✅ |
| Self-review | ❌ | ❌ | ✅ |
| Hallucination reduction | Low | Medium | High |
| Accuracy | Medium | High | Very High |

---

# 10. Learning Outcomes

After completing this project, I learned:

- Prompt Engineering
- Chain-of-Thought Prompting
- Logical Reasoning
- AI Self-Verification
- Hallucination Reduction
- Critical Thinking
- Prompt Optimization

---

# 11. Challenges Faced

Some AI models attempted to explain the puzzle immediately without verifying the arithmetic.

Designing a structured prompt that required verification before answering significantly improved the reasoning quality.

---

# 12. Conclusion

This project demonstrates that prompt design has a significant impact on AI reasoning quality.

Using a Chain-of-Thought prompt with structured verification helped the AI analyze the Missing Dollar Puzzle systematically, detect the misleading arithmetic, avoid logical errors, and provide a reliable explanation.

The project also showed that self-verification is an effective technique for reducing hallucinations and improving response accuracy in Large Language Models.

---

# 13. Future Improvements

Future work may include:

- Testing the prompt on different AI models.
- Evaluating more logical puzzles.
- Measuring response consistency.
- Creating a benchmark dataset for reasoning tasks.
- Comparing multiple prompting techniques.

---

# 14. References

1. DecodeLabs Prompt Engineering Project 2 Guidelines
2. OpenAI Prompt Engineering Concepts
3. Anthropic Prompt Engineering Guide
4. Google Prompt Engineering Best Practices
