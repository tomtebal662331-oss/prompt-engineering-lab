Prompt Engineering Lab

How Prompt Design Affects Generative AI Output Quality

1. Project Overview

This project is a controlled Prompt Engineering experiment designed to investigate how different prompt strategies affect the quality of Generative AI outputs.

We compare three prompt approaches:

1. Zero-shot Prompt
2. Few-shot Prompt
3. Refined Prompt

The three prompts are tested on the same task, using the same input and the same AI model, so that the effect of prompt design can be evaluated fairly.

---

2. Project Objective

The objective of this experiment is to answer the following question:

«How does changing the structure and level of detail of a prompt affect the quality of a Generative AI response?»

The experiment is designed to:

- Compare Zero-shot, Few-shot, and Refined prompting.
- Observe how prompt structure affects the generated output.
- Evaluate the outputs using defined quality criteria.
- Identify which prompting strategy performs best for the selected task.
- Document the evidence, results, and lessons learned.

---

3. Experiment Use Case

Scenario

The AI model is asked to create a 7-day cultural trip across:

- Italy
- France
- Spain

User Profile

- Trip Type: Cultural
- Budget: Medium
- Target User: Young Adult Traveler
- Interests: History, Museums, Local Food, Architecture

Core Task

Generate a practical 7-day cultural travel plan covering the selected countries and matching the specified user preferences and constraints.

---

4. Experimental Design

To make the comparison fair, the experiment keeps the following conditions constant:

Variable| Controlled Value
Use Case| 7-day cultural trip
Destinations| Italy, France, Spain
Budget| Medium
Target User| Young Adult Traveler
Interests| History, Museums, Local Food, Architecture
AI Model| Same model for all tests
Input| Same task conditions
Evaluation Criteria| Same criteria

The only major variable being changed is the prompt strategy.

Experiment Flow

Same Use Case
      │
      ├── Zero-shot Prompt
      │        ↓
      │      Output
      │
      ├── Few-shot Prompt
      │        ↓
      │      Output
      │
      └── Refined Prompt
               ↓
             Output
               │
               ▼
        Evaluation & Comparison
               │
               ▼
        Reflection & Conclusion

---

5. Prompt Strategies

5.1 Zero-shot Prompt

The AI receives the task directly without examples.

Purpose:

Establish a simple baseline and observe what the model produces from a direct instruction.

Location:

"prompts/zero-shot.md"

---

5.2 Few-shot Prompt

The AI receives examples before being asked to solve the target task.

Purpose:

Test whether examples help the model understand the expected pattern, structure, and style of the response.

Location:

"prompts/few-shot.md"

---

5.3 Refined Prompt

The prompt provides more explicit guidance, including structured requirements such as:

- Role
- Context
- Task
- Constraints
- Output Format
- Quality Criteria

Purpose:

Test whether explicit context, constraints, and formatting requirements produce a more relevant, complete, structured, and useful response.

Location:

"prompts/refined.md"

---

6. Outputs

The complete AI responses are stored without manually rewriting the generated content.

Strategy| Output
Zero-shot| "outputs/zero-shot.md"
Few-shot| "outputs/few-shot.md"
Refined| "outputs/refined.md"

These files represent the actual results used in the evaluation.

---

7. Evaluation Method

Each output is evaluated using five criteria.

Every criterion is scored from 1 to 5.

Criterion| Meaning
Relevance| How well the response addresses the requested task
Completeness| How fully the required information is provided
Structure| How clearly and logically the response is organized
Constraint Adherence| How well the response follows the specified requirements
Usefulness| How practical and helpful the response is for the target user

Evaluation Formula

Total Score = Sum of all five criteria

Maximum Score = 25

The detailed evaluation is available in:

"evaluation/evaluation.md"

---

8. Experimental Results

The current evaluation shows:

Prompt Strategy| Score
Zero-shot| 17 / 25
Few-shot| 19 / 25
Refined| 25 / 25

Result

Based on the current evaluation, the Refined Prompt achieved the highest score.

However, this conclusion is based on the measured results of this experiment rather than assuming in advance that the Refined Prompt would perform best.

---

9. Evidence

The project includes supporting evidence for the experiment and evaluation.

Evidence may include:

- AI-generated outputs
- Screenshots
- Evaluation observations
- Comparative results

Visual evidence is stored in:

"assets/screenshots/"

---

10. Reflection

The Reflection explains:

- How the outputs changed across the three prompt strategies.
- How prompt design affected response quality.
- Which strategy performed best.
- Why the results differed.
- What the team learned from the experiment.
- What trade-offs were observed.

Location:

"reflection/reflection.md"

---

11. Presentation

The technical presentation summarizes the complete experiment.

It covers:

1. Project Objective
2. Problem Statement
3. Experiment Design
4. Prompt Evolution
5. Results
6. Evidence
7. Conclusion

Location:

"presentation/"

---

12. Repository Structure

prompt-engineering-lab/
│
├── README.md
│
├── prompts/
│   ├── zero-shot.md
│   ├── few-shot.md
│   └── refined.md
│
├── outputs/
│   ├── zero-shot.md
│   ├── few-shot.md
│   └── refined.md
│
├── evaluation/
│   └── evaluation.md
│
├── reflection/
│   └── reflection.md
│
├── presentation/
│   └── slides.md
│
└── assets/
    └── screenshots/

What each folder contains

"prompts/"
The exact prompts used in the experiment.

"outputs/"
The original AI responses generated from each prompt.

"evaluation/"
The scoring, comparison, and evidence used to evaluate the outputs.

"reflection/"
The interpretation of the results and lessons learned.

"presentation/"
The technical presentation of the experiment.

"assets/screenshots/"
Screenshots and visual evidence supporting the experiment.

---

13. Team Roles

Role| Responsibility
Project Lead| Repository, coordination, workflow, integration, and Final QA
Prompt Engineer| Design and document Zero-shot, Few-shot, and Refined prompts
AI Evaluation| Execute experiments, preserve outputs, and evaluate results
Research & Presentation Engineer| Analyze findings, write Reflection, and prepare Presentation

Collaboration Workflow

Project Lead
     ↓
Prompt Engineer
     ↓
AI Evaluation
     ↓
Research & Presentation
     ↓
Project Lead
     ↓
Final QA
     ↓
Submission

Each stage must be completed and reviewed before the next stage begins.

---

14. Quality Assurance

Before submission, the Project Lead verifies:

- [ ] All three prompts are present.
- [ ] All three outputs are present.
- [ ] The same experimental conditions were used.
- [ ] The evaluation criteria are applied consistently.
- [ ] Scores match the evaluation evidence.
- [ ] Reflection matches the actual results.
- [ ] Presentation matches the documented experiment.
- [ ] Required screenshots/evidence are available.
- [ ] Repository structure is complete and organized.
- [ ] No required deliverable is missing.

The project is considered ready for submission only after the Final QA is completed.

---

15. Key Finding

This experiment demonstrates that prompt design can significantly affect the quality of Generative AI outputs.

The results from this experiment show an improvement from:

Zero-shot  →  17/25
Few-shot   →  19/25
Refined    →  25/25

The experiment therefore provides practical evidence that adding examples, context, constraints, and explicit output requirements can improve response quality for the selected task.

---

16. Important Note

This project evaluates prompt strategies for one specific use case and one controlled experiment.

The results should therefore be interpreted as evidence for this experiment, not as a universal claim that one prompting strategy will always outperform another across all AI tasks.

---

17. Project Status

Status: Finalizing

Experiment: Prompt Engineering Comparison
Evaluation: Completed
Reflection: Completed
Presentation: In Progress / Final Review

---

18. Quick Start for a New Reader

Someone opening this repository for the first time can follow this order:

1. Read README.md
        ↓
2. Open prompts/
        ↓
3. Compare the three prompt strategies
        ↓
4. Open outputs/
        ↓
5. Compare the generated responses
        ↓
6. Open evaluation/
        ↓
7. Review the scores and evidence
        ↓
8. Open reflection/
        ↓
9. Understand the findings
        ↓
10. Open presentation/
        ↓
11. Review the complete experiment summary

No additional explanation from the project team should be required to understand the experiment.- **Key Findings**: Summary of important discoveries
- **Best Practices**: Documented recommendations and patterns
- **Lessons Learned**: Insights for future experiments
- **Improvement Suggestions**: Recommendations for optimization

### 4. Presentations & Assets
- **Presentation Decks**: Slides for stakeholder communication
- **Visual Assets**: Screenshots, diagrams, and infographics
- **Executive Summaries**: High-level overviews of key findings
- **Technical Reports**: Detailed documentation for reference

### 5. Knowledge Repository
- **Prompt Templates**: Reusable prompt structures
- **Technique Guide**: Documentation of prompt engineering techniques
- **Case Studies**: Real-world examples and applications
- **FAQ & Troubleshooting**: Common questions and solutions

## Project Structure

```
prompt-engineering-lab/
├── README.md                 # Project overview and documentation
├── prompts/                  # Experimental prompts collection
│   └── [experiment folders]
├── outputs/                  # Model outputs and results
│   └── [experiment folders]
├── evaluation/               # Analysis and evaluation reports
│   └── [analysis files]
├── reflection/               # Insights and best practices
│   └── [reflection documents]
├── presentation/             # Presentation materials
│   └── [presentation files]
└── assets/
    └── screenshots/          # Visual assets and screenshots
```

## Getting Started

1. Review this README and understand the project objectives
2. Check the project structure and navigate to relevant folders
3. Review existing experiments and results in `outputs/` and `evaluation/`
4. Submit new experiments following the methodology guidelines
5. Contribute to knowledge sharing through documentation

## Contributing

When contributing to this project:
1. Follow the established experiment methodology
2. Document all prompts and approaches clearly
3. Maintain consistent naming and organization
4. Include comprehensive analysis and findings
5. Update relevant documentation

## Version History

- **v1.0** (Initial Release): Project structure and documentation established

---
