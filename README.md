# EXP-2-PROMPT-ENGINEERING-

## Aim: 
Comparative Analysis of different types of Prompting patterns and explain with Various Test Scenarios

Experiment:
Test and compare how different pattern models respond to various prompts (broad or unstructured) versus basic prompts (clearer and more refined) across multiple scenarios. 
Analyze the quality, accuracy, and depth of the generated responses.


## Algorithm:

```
Step 1: Start.
Step 2: Define prompting patterns to be tested:
    a. Zero-Shot Prompting
    b. Few-Shot Prompting
    c. Chain-of-Thought Prompting
    d. Role-Based Prompting
    e. Refined/Instructional Prompting

Step 3: Select test scenarios:
    a. Broad/Unstructured prompt (Explain AI).
    b. Problem-solving prompt (Worker efficiency problem).
    c. Creative prompt (Story about a robot learning friendship).

Step 4: Apply each prompting pattern to the chosen scenarios.

Step 5: Record responses for quality, accuracy, depth, creativity, and flexibility.

Step 6: Compare performance using both tabular analysis and visual chart.

Step 7: Identify best performing prompt type for each scenario.

Step 8: Summarize findings.

Step 9: End.
```

## Output:
```
1. Tabular Comparison
Scenario / Prompt Type	Zero-Shot	Few-Shot	Chain-of-Thought	Role-Based	Refined
Explain AI	Generic, vague	Some structure	Detailed but verbose	Audience-specific	Clear, structured
Worker Problem	Direct but no steps	Example-based correct	Step-by-step accurate	Tutor-style	Structured + accurate
Robot Story	Simple, flat	Better style	Logical but less creative	Engaging, rich	Detailed, emotional
2. Visual Comparison (Radar Chart)

The radar chart below compares five prompting strategies across clarity, accuracy, depth, creativity, and flexibility.

Zero-Shot: Lowest coverage (basic, vague).

Few-Shot: Balanced but average across all.

Chain-of-Thought: High accuracy and depth (best for reasoning).

Role-Based: High creativity and clarity (best for stories/explanations).

Refined: Overall best performance with consistently high scores.

<img width="1320" height="1229" alt="image" src="https://github.com/user-attachments/assets/2ed916c6-c16e-4985-b90c-6dc65fecffd1" />
```

## Result:
```
Zero-Shot Prompting is quick but produces shallow and generic answers.

Few-Shot Prompting improves structure when examples are available, but remains average in performance.

Chain-of-Thought Prompting achieves highest accuracy and depth, making it best for reasoning and problem-solving.

Role-Based Prompting delivers creative, contextual, and engaging outputs, suitable for teaching and storytelling.
```
Refined Prompting provides the most balanced, high-quality outputs across all test scenarios, making it the most reliable overall.
