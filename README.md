# Task 01: Zero-Shot vs Few-Shot Prompt Engineering Showdown

## 📋 Project Overview

This project demonstrates the fundamental difference between zero-shot and few-shot prompting in generative AI. We tested three major AI models (Claude, ChatGPT, and Gemini) on a customer support message classification task using both approaches.

**Repository:** `neurofive-prompt-engineering-task-01`

## 🎯 Objective

To understand how providing examples (few-shot) versus providing no examples (zero-shot) affects AI model accuracy and reliability in classification tasks.

## 📊 Task Description

**Problem:** Classify 10 customer support messages into three categories:
- **Complaint** - Messages expressing dissatisfaction
- **Question** - Messages asking for information or help
- **Praise** - Messages expressing satisfaction or compliments

## 🔧 Methodology

### Zero-Shot Approach
Prompt with only instruction and no examples:
```
Classify the following customer support messages into one of three categories: 
"Complaint", "Question", or "Praise".

[10 messages]

For each message, provide only the classification.
```

### Few-Shot Approach
Prompt with instruction + 3 labeled examples:
```
Classify the following customer support messages into one of three categories: 
"Complaint", "Question", or "Praise".

Examples:
- "Your product is amazing!" → Praise
- "How do I change my settings?" → Question
- "This is broken and I'm furious!" → Complaint

[10 messages]

For each message, provide only the classification.
```

## 📈 Results

| AI Model | Zero-Shot Accuracy | Few-Shot Accuracy |
|----------|-------------------|------------------|
| Claude   | 100% (10/10)      | 100% (10/10)     |
| ChatGPT  | 100% (10/10)      | 100% (10/10)     |
| Gemini   | 100% (10/10)      | 100% (10/10)     |

## 💡 Key Findings

1. **All models achieved perfect accuracy** in both zero-shot and few-shot scenarios for this straightforward classification task.

2. **Few-shot prompting is still superior** because:
   - Reduces ambiguity in complex tasks
   - Increases consistency and reliability
   - Provides clearer expectations
   - Essential for production systems

3. **Zero-shot performance was strong**, indicating modern LLMs have excellent reasoning capabilities, but examples always improve clarity.

## 📝 Files Included

- `TASK_01_RESULTS.txt` - Detailed results and analysis table
- `README.md` - This file
- `PROMPTS.txt` - Complete prompts used
- `ANALYSIS.txt` - Detailed analysis and insights

## 🎓 Learning Outcome

This task confirms the core prompt engineering principle: **Always provide examples when precision matters.** While zero-shot prompting can work, few-shot prompting is the industry best practice for production applications.

## 📌 Recommendations

For real-world applications:
- Always use few-shot prompting for consistent results
- Provide 2-5 diverse examples covering edge cases
- Test on multiple AI models to ensure reliability
- Monitor outputs and refine examples based on failures


## 📅 Date

Week 1 - Generative AI & Prompt Engineering Fundamentals

---

**Status:** ✅ Completed

