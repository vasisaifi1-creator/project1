# Prompting Fundamentals on Real Tasks v2 (FL-02)

**Name:** Mohd Vasi Saifi  
**Program:** B.Tech (Hons.) Artificial Intelligence & Machine Learning  
**University:** SDGI Global University, Ghaziabad  
**GitHub:** https://github.com/vasisaifi1-creator  
**Date:** July 2026

---

# Objective

The objective of this assignment is to improve an AI prompt through multiple iterations by applying prompt engineering techniques. The selected real-world task is designing a professional AI portfolio website that can be used to showcase my skills, projects, certifications, and internship work to recruiters.

---

# Real Task

Create a modern AI Portfolio Website for internship applications.

The website should:

- Showcase my technical skills
- Present AI and web development projects
- Display certifications
- Include resume download
- Provide contact information
- Help recruiters evaluate my abilities

---

# Baseline Prompt (Naïve Prompt)

```
Build an AI portfolio website.
```

## AI Output (Summary)

The AI generated a simple response suggesting pages such as Home, About, Projects, and Contact. The response was generic and lacked personalization, technical guidance, and implementation details.

### Observation

The prompt was too short and did not explain:

- Who the website is for
- What technologies to use
- What information should be included
- The expected output format

---

# Iteration 1 — Technique: Role Assignment

## Prompt

```
You are an experienced Full Stack Web Developer.

Help me build a professional AI portfolio website.
```

## Output Summary

The AI responded like an experienced developer and suggested:

- Responsive layout
- Professional navigation
- Hero section
- Skills section
- Project cards
- Contact page

### What Changed

Assigned the AI a professional role.

### Why

Giving the AI a role helps it answer from the perspective of an expert.

### Output Difference

The advice became more practical and technically accurate.

---

# Iteration 2 — Technique: Add Context

## Prompt

```
You are an experienced Full Stack Web Developer.

Create an AI portfolio for Mohd Vasi Saifi.

I am currently studying B.Tech (Hons.) Artificial Intelligence and Machine Learning at SDGI Global University.

The purpose of this website is to secure AI and software engineering internships.
```

## Output Summary

The AI produced personalized content including:

- Student introduction
- Education details
- Career objective
- Technical skills
- AI projects
- Resume section

### What Changed

Added personal information and project context.

### Why

Context enables the AI to create customized responses.

### Output Difference

The portfolio became more realistic and personalized.

---

# Iteration 3 — Technique: Define the Audience

## Prompt

```
Design the portfolio specifically for recruiters, internship mentors, and hiring managers.

Focus on demonstrating practical skills instead of generic descriptions.
```

## Output Summary

The AI changed its writing style.

Instead of simply listing skills, it emphasized:

- Real projects
- GitHub repositories
- Technical achievements
- Internship readiness

### What Changed

Specified the audience.

### Why

The audience determines tone and priorities.

### Output Difference

The response became more persuasive and recruiter-focused.

---

# Iteration 4 — Technique: Specify Output Structure

## Prompt

```
Generate the complete portfolio with the following sections:

1. Home
2. About
3. Skills
4. Projects
5. Certifications
6. Resume
7. Contact

Provide HTML, CSS, JavaScript, and explain each section.
```

## Output Summary

The AI organized the response clearly and produced:

- HTML layout
- CSS styling recommendations
- JavaScript functionality
- Navigation design
- Resume button
- Contact form

### What Changed

Specified the required output format.

### Why

A structured request produces a structured response.

### Output Difference

The result became implementation-ready.

---

# Iteration 5 — Technique: Constraints & Quality Criteria

## Prompt

```
Act as a Senior Full Stack AI Engineer.

Create a production-ready AI portfolio website.

Requirements:

- HTML5
- CSS3
- JavaScript
- Responsive Design
- Mobile Friendly
- SEO Friendly
- Fast Loading
- Clean Code
- Accessibility Best Practices
- GitHub Ready

Include:

- Hero Section
- About
- Skills
- Projects
- Certifications
- Resume Download
- Contact Form
- GitHub
- LinkedIn

Use modern UI design with animations and comments inside the code.
```

## Output Summary

The AI generated a professional solution with:

- Modern interface
- Responsive design
- Professional color palette
- Smooth scrolling
- Clean project cards
- Better accessibility
- Production-quality recommendations

### What Changed

Added quality requirements and constraints.

### Why

Constraints improve consistency and output quality.

### Output Difference

The response became significantly more detailed and professional.

---

# Comparison: Claude vs ChatGPT

| Feature | Claude | ChatGPT |
|----------|----------|----------|
| Explanation Quality | Excellent | Excellent |
| Technical Detail | High | Very High |
| Organization | Good | Excellent |
| Code Structure | Good | Excellent |
| Readability | Excellent | Excellent |
| Best Use | Brainstorming and reasoning | Coding and structured implementation |

## Observation

Claude produced thoughtful explanations and reasoning, while ChatGPT generated more structured, implementation-ready content. Combining insights from both resulted in a stronger final solution.

---

# Final Reusable Prompt

```
Act as an experienced Full Stack AI Developer and UI/UX Designer.

Design a professional AI Portfolio Website.

Purpose:
Showcase technical skills, AI projects, certifications, education, and internship experience.

Audience:
Recruiters, internship mentors, and software engineering hiring managers.

Requirements:

• Responsive Design
• HTML5
• CSS3
• JavaScript
• Mobile Friendly
• SEO Optimized
• Accessibility Best Practices
• Fast Loading
• Modern UI
• Clean Code

Website Sections:

- Home
- About Me
- Skills
- Projects
- Certifications
- Resume
- Contact

Generate production-ready code with comments.

Explain important implementation decisions.

Recommend improvements where appropriate.
```

---

# Lessons Learned

This assignment demonstrated that small improvements in prompt design can significantly improve AI-generated responses.

The most effective techniques were:

- Role Assignment
- Context
- Audience Definition
- Structured Output
- Quality Constraints

These techniques transformed a vague request into a professional, implementation-ready solution.

---

# Reflection

Initially, the AI produced a very generic answer because the prompt lacked detail. By improving one aspect at a time, the quality of the responses improved dramatically. This process showed that prompt engineering is an iterative skill that requires clarity, context, and well-defined expectations.

---

# Conclusion

The final reusable prompt consistently generates professional AI portfolio website recommendations suitable for internship applications. This exercise improved my understanding of prompt engineering and demonstrated how structured prompts produce significantly better AI outputs.