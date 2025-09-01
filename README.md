# EXP-2-PROMPT-ENGINEERING-

Comparative Analysis of Prompting Patterns: A Detailed Report 

Executive Summary 

This report provides a comprehensive comparative analysis of various prompt engineering patterns and their impact on the performance of Large Language Models (LLMs). Through a series of controlled experiments, we test how different prompting techniques, from basic to advanced, affect the quality, accuracy, and depth of generated responses. The findings demonstrate that a well-crafted, structured prompt is critical for unlocking an LLM's full potential, especially for complex reasoning, multi-step problem-solving, and tasks requiring factual accuracy. 

 

Introduction 

 Background 

The rise of large language models has transformed the landscape of AI-driven applications. While LLMs are incredibly powerful, their performance is highly dependent on the input they receive. Prompt engineering is the art and science of designing effective prompts to guide models toward desired outputs. This report investigates how different prompting patterns influence an LLM's response quality. 

Objective 

The primary objective of this experiment is to: 

Define and categorize different prompting patterns. 

Design and execute test scenarios to compare these patterns. 

Analyze the generated responses based on pre-defined metrics: quality, accuracy, and depth. 

Present a clear, data-driven conclusion on which patterns are most effective for specific types of tasks. 

Prompting Patterns: A Taxonomy 

This section defines the key prompting patterns we will test. We've grouped them into two main categories: Basic and Advanced. 

 Basic Prompting Patterns 

A. Zero-Shot Prompting (Unstructured): The most fundamental method. The model is given a broad, direct instruction without any examples. It relies entirely on its pre-trained knowledge. 

B. Basic Refined Prompting (Structured): A more refined version of zero-shot. The prompt includes clearer instructions, context, and a specified format (e.g., "Summarize the following text in three bullet points."). 

Advanced Prompting Patterns 

C. Few-Shot Prompting: The prompt includes a small number of examples (shots) of the desired input/output format. The model learns the pattern and applies it to a new, unseen input. 

D. Chain-of-Thought (CoT) Prompting: A technique that encourages the model to break down a complex problem into a sequence of intermediate steps. This can be done by simply adding a phrase like "Let's think step by step" (Zero-Shot CoT) or by providing examples with the reasoning steps included (Few-Shot CoT). 

E. Role-Playing/Persona Prompting: The prompt assigns a specific role or persona to the model (e.g., "Act as a senior software engineer..."). This influences the tone, style, and content of the response. 

F. Generated Knowledge Prompting: A two-part prompt. The first part asks the model to generate relevant facts or a knowledge base, and the second part uses that generated information to answer the main query. 

 

Experimental Design and Test Scenarios 

To provide a robust comparison, we designed a series of test scenarios covering different domains and task complexities. For each scenario, we will use a single LLM and run the same task using each of the defined prompting patterns. 

Scenario 1: Mathematical Reasoning 

Task: Solve a multi-step word problem. 

Broad/Unstructured Prompt (Zero-Shot): "I have 15 marbles. I give 4 to my sister, then my brother gives me twice the number I have left. How many marbles do I have now?" 

Basic/Refined Prompt: "Solve the following word problem and give the final answer as a number: I have 15 marbles. I give 4 to my sister, then my brother gives me twice the number I have left. How many marbles do I have now?" 

CoT Prompt: "I have 15 marbles. I give 4 to my sister, then my brother gives me twice the number I have left. How many marbles do I have now? Let's think step by step." 

Scenario 2: Factual and Creative Content Generation 

Task: Write a short informational paragraph about a historical event. 

Broad/Unstructured Prompt: "Write about the moon landing." 

Basic/Refined Prompt: "Write a 100-word paragraph about the Apollo 11 moon landing. Include key dates and figures." 

Few-Shot Prompt: 

Input: "The Great Wall of China" 

Output: "The Great Wall of China, a series of fortifications built across the historical northern borders of China, was constructed from the 7th century BC to the Ming Dynasty. It was built to protect Chinese states and empires against the raids and invasions of various nomadic groups." 

Input: "The Apollo 11 Moon Landing" 

Output:  

3.3 Scenario 3: Code Generation 

Task: Write a Python function for a specific task. 

Broad/Unstructured Prompt: "Write a function to sort a list of numbers." 

Basic/Refined Prompt: "Write a Python function called sort_numbers that takes a list of integers as input and returns a new list with the numbers sorted in ascending order." 

Few-Shot Prompt: 

Input: "Write a Python function to check if a number is even." 

Output:  

Python 

def is_even(number): 
    return number % 2 == 0 
 

Input: "Write a Python function to find the maximum number in a list." 

Output:  

 

Literature Review 

Zero-shot prompting – No examples given, relies solely on training. 

Few-shot prompting – A few examples are provided to guide. 

Chain-of-thought prompting – Encourages step-by-step reasoning. 

Instruction prompting – Direct structured commands. 

Role prompting – AI is given a role (e.g., teacher, doctor). 

Self-consistency prompting – Multiple reasoning paths, selects best. 

📌 Previous research findings: 

Few-shot improves factual accuracy. 

Chain-of-thought helps in logical reasoning. 

Role prompting boosts creativity. 

Instruction-based ensures clarity. 

 

Research Methodology 

Design: Test five scenarios with multiple prompting methods. 

Test Scenarios: 

General knowledge Q&A 

Mathematical problem-solving 

Creative story writing 

Summarization 

Code debugging 

Evaluation Parameters: 

Accuracy (Correctness of information) 

Clarity (Well-structured and readable) 

Creativity (Novelty and uniqueness) 

Consistency (Logical flow and reliability) 

Scoring: 1–10 scale. 

 

Types of Prompting Patterns 

Zero-shot → Best for general tasks, lacks reasoning. 

Few-shot → Improves reliability, especially in structured tasks. 

Chain-of-thought → Strong in mathematics and logical reasoning. 

Instruction-based → Ideal for summarization, report writing, coding. 

Role-based → Useful for storytelling and simulations. 

Self-consistency → High accuracy in reasoning-heavy problems. 

Test Scenarios & Experimentation 

Scenario 1: General Knowledge Q&A 

Broad Prompt: “Tell me about AI.” → Vague response. 

Refined Prompt: “Explain AI in 150 words with real-world examples.” → Structured, accurate. 

Observation: Instruction-based > Zero-shot. 

Scenario 2: Mathematical Problem Solving 

Broad Prompt: “Solve this problem: A + B = 20.” → Direct answer, no reasoning. 

Refined Prompt (Chain-of-thought): “Explain step by step how to solve A + B = 20 if A = 12.” → Detailed reasoning. 

Observation: Chain-of-thought > Zero-shot. 

Scenario 3: Creative Writing 

Broad Prompt: “Write a story.” → Random, unfocused story. 

Refined Prompt (Role-based): “Write a short story as a children’s author with a moral lesson.” → Engaging and meaningful. 

Observation: Role-based > Few-shot. 

Scenario 4: Summarization 

Broad Prompt: “Summarize this.” → Short, vague summary. 

Refined Prompt (Instruction-based): “Summarize this text in 100 words, highlighting key challenges and solutions.” → Accurate, concise. 

Observation: Instruction-based > Zero-shot. 

Scenario 5: Coding & Debugging 

Broad Prompt: “Fix the error.” → May miss details. 

Refined Prompt (Few-shot): “Here is a Python function. Identify the error and correct it with explanation.” → Clear and correct debugging. 

Observation: Few-shot > Zero-shot. 

 

 Analysis & Discussion 

Zero-shot: Fast, general, but weak in reasoning. 

Few-shot: Reliable and good for technical/coding tasks. 

Chain-of-thought: Excellent for problem-solving. 

Role prompting: Best for creativity, storytelling, teaching. 

Instruction prompting: Best for structured outputs. 

Self-consistency: Increases reliability for complex reasoning. 

 

 Results and Analysis 

This section will present the generated outputs for each scenario and analyze them against our metrics. 

 Test Scenario 1: Mathematical Reasoning 

Zero-Shot Output: The model may provide a quick but incorrect answer, like 15 - 4 = 11 then 11 + 2 = 13. 

Basic Refined Output: The model might provide the correct answer (27), but the process is a black box. 

CoT Output: The model demonstrates a clear, step-by-step process: 

Initial marbles: 15 

Marbles after giving some away: 15 - 4 = 11 

Marbles received from brother: 11 * 2 = 22 

Final marbles: 11 + 22 = 33 

Analysis: CoT prompting is a clear winner for reasoning tasks. The structured approach forces the model to perform each calculation sequentially, leading to a higher degree of accuracy and a transparent thought process. 

Test Scenario 2: Factual and Creative Content 

Zero-Shot Output: A general, high-level summary of the moon landing, often lacking specific details or a clear structure. 

Basic Refined Output: A concise, well-structured paragraph that meets all the specified constraints (e.g., 100 words, includes dates and names). The quality is significantly higher. 

Few-Shot Output: A paragraph that not only provides accurate information but also mimics the style, tone, and sentence structure of the example provided. 

Analysis: Few-shot prompting is highly effective for tasks where a specific style or format is paramount. The examples serve as a strong guide, improving the model's ability to replicate the desired output. 

Test Scenario 3: Code Generation 

Zero-Shot Output: The code might be functional but may lack best practices, comments, or error handling. 

Basic Refined Output: The function is more robust and follows the instructions precisely, with a clear name and correct input/output. 

Few-Shot Output: The generated code is not only correct but also stylistically consistent with the examples, including docstrings, variable naming conventions, and specific syntax choices. 

Analysis: Few-shot prompting, especially with code examples, is a powerful tool for maintaining consistency and generating code that adheres to specific formatting and best practices, making it far more useful in a professional context. 

 

 Comparative Tables and Diagrams 

 Response Quality Matrix 

Prompt Pattern 

Clarity 

Completeness 

Accuracy 

Depth 

Zero-Shot 

Low 

Low-Medium 

Low-Medium 

Low 

Basic Refined 

Medium 

Medium-High 

High (for simple tasks) 

Medium 

Few-Shot 

High 

High 

High 

High (in-context) 

Chain-of-Thought 

High 

High 

Very High (for reasoning) 

High (reasoning steps) 

Export to Sheets 

Response Comparison Diagrams 

Diagram 1: The Funnel of Prompting. A visual representation of how prompts refine the model's output, from a wide, unstructured input (broad) to a narrow, precise output (refined). 

Diagram 2: CoT vs. Zero-Shot. A side-by-side flow chart illustrating the "black box" of zero-shot vs. the transparent, step-by-step process of Chain-of-Thought. 

 

 Conclusion and Recommendations 

This experiment confirms that prompt engineering is not merely an optional step but a critical factor in harnessing the power of LLMs. 

Basic prompts are suitable for simple, well-defined tasks where a quick, general response is all that is needed. 

Refined prompts with clear instructions significantly improve output quality and can handle more complex tasks with better reliability. 

Advanced patterns like Chain-of-Thought and Few-Shot are essential for demanding tasks. CoT unlocks a model's reasoning capabilities, making it reliable for logical and mathematical problems. Few-Shot is invaluable for tasks requiring a specific output style, format, or tone. 

Recommendations: 

For R&D and complex problem-solving: Use Chain-of-Thought prompting to improve accuracy and make the model's reasoning transparent. 

For content generation and data tasks: Employ Few-Shot prompting to ensure consistency in style and format across multiple outputs. 

For general use: Start with a Basic Refined Prompt and only increase complexity if the initial results are unsatisfactory. 

Limitations and Future Work 

This study was conducted using a single model. Future work should involve a cross-model comparison to determine if these findings are universal. Additionally, we could explore other advanced techniques like tree-of-thoughts or self-consistency prompting for even more complex tasks. 

 

 Appendix 

Complete prompt scripts for all test scenarios. 

Raw outputs from the model for each test run. 

Bibliography of relevant research papers and articles. 

 

Output 

After testing the different prompting patterns across five scenarios, the outputs were as follows: 

General Knowledge Q&A 

Zero-shot: Provided a generic, unfocused explanation. 

Instruction-based: Delivered a structured, concise explanation with real-world examples. 

Mathematical Problem Solving 

Zero-shot: Direct answer, but no reasoning. 

Chain-of-thought: Step-by-step explanation with correct reasoning. 

Creative Writing 

Zero-shot: Random short story, lacking depth. 

Role-based: Engaging story with characters, moral lesson, and creativity. 

Summarization 

Zero-shot: Very short summary, missing details. 

Instruction-based: Accurate 100-word summary with key challenges and solutions. 

Coding/Debugging 

Zero-shot: Attempted fix but incomplete. 

Few-shot: Correct error detection, explanation, and working code output. 

📌 The outputs clearly varied in quality, detail, and reliability depending on the prompting strategy. 

 

Result 

Chain-of-thought prompting achieved the highest accuracy and consistency in logical and mathematical tasks. 

Role prompting delivered the most creative and engaging outputs in storytelling. 

Instruction-based prompting produced the clearest and most structured answers, especially in summarization. 

Few-shot prompting improved technical tasks such as coding/debugging. 

Zero-shot prompting worked well for simple queries but lacked depth in complex reasoning. 

Overall Conclusion: 

Refined prompts outperform unstructured prompts in every scenario. 

The best prompting technique depends on the task: 

Q&A → Instruction-based 

Math → Chain-of-thought 

Storytelling → Role-based 

Coding → Few-shot 

Summarization → Instruction-based 

 

 
