# FL-04: Ship an Automation Workflow v2

**Name:** Mohd Vasi Saifi  
**Track:** General AI Fluency  
**Week:** 4  
**Assignment:** FL-04 – Ship an Automation Workflow v2

---

# Workflow Title

## AI Study Notes Generator

### Objective

The purpose of this workflow is to automatically generate well-structured study notes from any technical topic using ChatGPT. The workflow reduces manual effort, improves consistency, and saves time while still allowing a human to review the final output for accuracy.

---

# Workflow Diagram

```
User selects a topic
        │
        ▼
Step 1: Research the topic
        │
        ▼
Step 2: Generate beginner-friendly explanation
        │
        ▼
Step 3: Create interview questions
        │
        ▼
Step 4: Format into study notes
        │
        ▼
Step 5: Human review
        │
        ▼
Final study notes
```

---

# Workflow Description

This workflow converts a single topic into complete study notes using multiple AI-assisted steps. Instead of manually searching, summarising, and formatting information, the AI performs each stage in sequence.

---

# Step 1 – Research

### Goal

Collect accurate information about the selected topic.

### Tool

ChatGPT

### Prompt

```
Research the topic "<TOPIC>" and explain its important concepts, applications, advantages and disadvantages.
```

### Input

Topic Name

Example:

```
Machine Learning
```

### Output

Detailed explanation of the topic.

---

# Step 2 – Simplify

### Goal

Convert the explanation into simple language.

### Tool

ChatGPT

### Prompt

```
Summarize the topic using simple English so that a beginner can understand it easily.
```

### Output

Easy-to-read summary.

---

# Step 3 – Interview Questions

### Goal

Prepare interview questions for revision.

### Tool

ChatGPT

### Prompt

```
Generate 10 interview questions with short answers based on the topic.
```

### Output

Interview preparation material.

---

# Step 4 – Format Notes

### Goal

Create clean study notes.

### Tool

ChatGPT

### Prompt

```
Format the complete content into markdown with headings, bullet points, tables where useful and a conclusion.
```

### Output

Professional study notes.

---

# Step 5 – Human Review

### Goal

Verify correctness before final use.

### Checklist

- Verify technical facts
- Correct grammar
- Improve formatting
- Remove duplicate information
- Ensure examples are correct

---

# Workflow Summary

| Step | Action | Tool | Output |
|------|--------|------|--------|
| 1 | Research topic | ChatGPT | Detailed explanation |
| 2 | Simplify content | ChatGPT | Beginner summary |
| 3 | Generate interview questions | ChatGPT | Q&A |
| 4 | Format notes | ChatGPT | Markdown notes |
| 5 | Human review | Human | Final verified notes |

---

# Five Test Runs

## Run 1

### Input

Machine Learning

### Output

- Topic researched successfully
- Summary generated
- 10 interview questions created
- Notes formatted correctly

**Status:** Success

**Time:** 8 minutes

---

## Run 2

### Input

Deep Learning

### Output

- Explanation generated
- Beginner summary created
- Interview questions produced
- Final notes formatted

**Status:** Success

**Time:** 8 minutes

---

## Run 3

### Input

Natural Language Processing

### Output

- Detailed explanation generated
- Summary completed
- Interview questions created
- Markdown notes prepared

**Status:** Success

**Time:** 9 minutes

---

## Run 4

### Input

Computer Vision

### Output

- Complete explanation generated
- Notes formatted successfully
- Interview questions included

**Status:** Success

**Time:** 8 minutes

---

## Run 5

### Input

Python Programming

### Output

- Beginner-friendly explanation
- Revision notes generated
- Interview questions prepared

**Status:** Success

**Time:** 7 minutes

---

# Time Comparison

| Activity | Manual Method | Workflow |
|----------|---------------:|---------:|
| Research | 15 min | 3 min |
| Summary | 10 min | 2 min |
| Interview Questions | 10 min | 2 min |
| Formatting | 5 min | 1 min |
| **Total Time** | **40 min** | **8 min** |

## Estimated Time Saved

Approximately **32 minutes** per topic.

---

# Failure Points

The workflow may not always provide the latest information for rapidly changing technologies.

If the prompt is unclear, the generated explanation may be incomplete.

Complex technical topics sometimes require additional clarification.

AI-generated answers should not be treated as perfect without verification.

---

# Human Review Required

A human reviewer should always:

- Check technical accuracy.
- Verify important facts.
- Improve grammar where needed.
- Remove incorrect information.
- Confirm examples are correct.
- Ensure the final notes are easy to understand.

---

# Advantages

- Saves time.
- Easy to repeat.
- Beginner friendly.
- Produces consistent notes.
- Requires no programming.
- Uses free AI tools.

---

# Limitations

- AI can occasionally make factual mistakes.
- Human verification is necessary.
- Some advanced topics need expert review.
- Quality depends on the prompt.

---

# Future Improvements

Possible future improvements include:

- Automatic PDF generation
- Flashcard creation
- Quiz generation
- Diagram generation
- Automatic citations
- Integration with GitHub Pages

---

# Conclusion

This workflow successfully automates the process of converting a technical topic into structured study notes. It divides the work into five clear stages: research, simplification, interview question generation, formatting, and human review. Compared with a fully manual approach, the workflow significantly reduces the time required while maintaining good quality. Human review remains an essential final step to ensure accuracy and reliability.

---

# Deliverables Checklist

- [x] Workflow selected
- [x] Workflow diagram included
- [x] Three or more workflow steps
- [x] Prompts documented
- [x] Five workflow runs completed
- [x] Time comparison included
- [x] Failure points documented
- [x] Human review explained
- [x] Complete walkthrough document
- [x] Final conclusion added