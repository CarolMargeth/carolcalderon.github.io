---
title: Style Checker App
image: /assets/images/checker.png
description: This project aims to enhance the performance of a language model (LLM) for a Clinical documentation task.
company: Personal project
date: 2024-10-13
layout: post
---

## Fine-tuning an LLM for Surgical Documentation

### Introduction

When I stumbled upon a repetitive task in my work - creating titles and descriptions for surgical moments - I realized there was an opportunity for improvement. This task, while crucial, was time-consuming and prone to inconsistencies. That's when I decided to explore the potential of fine-tuning a Large Language Model (LLM) to streamline this process.

The challenge was significant: I needed a model that could handle high variability in inputs, produce outputs tailored to our company's specific style, and cater to users with different technical backgrounds. Here you will find details of my journey through this project, from conception to deployment.

### Background

Before diving into the project, let me briefly explain what LLMs are and what fine-tuning means. 

Large Language Models (LLMs) are advanced AI systems trained on vast amounts of text data, capable of generating human-like text based on input prompts. Typically, we interact with LLMs through prompting - providing specific instructions or examples to guide the model's output.

Fine-tuning, on the other hand, involves further training an existing LLM on a specific dataset to specialize it for a particular task. This process can lead to better performance and more consistent outputs for targeted applications.

Before diving into fine-tuning, I researched the differences, advantages, and disadvantages between prompting and fine-tuning. Initial attempts with advanced prompting didn't yield satisfactory results, reinforcing my decision to pursue fine-tuning.

Also, in my initial exploration, I found that people performing the task frequently used LLMs to support their work, but the quality of results wasn't satisfactory. This observation led me to consider fine-tuning as a potential solution.

For my surgical documentation project, fine-tuning was an attractive option because:
- It allowed us to incorporate our company's specific style and terminology
- It could potentially handle the high variability in our inputs more effectively
- Fine-tuned models often require shorter, more efficient prompts
- It offered the possibility of improved consistency across different user skill levels

### Project Setup

To get started, I expected to use a tools like: 

- Python programming language
- Hugging Face Transformers library for working with LLMs
- Jupyter Notebooks for experimentation and analysis
- Git for version control
- Cloud platforms (e.g., AWS) for model training and deployment
- Web development frameworks (e.g., Flask, React) for creating a user interface

Each played a crucial role in different stages of the project.

### Fine-tuning Process

[Step 1]
Dataset preparation was a critical step. I gathered historical data from the surgical documentation, performed exploratory analysis to identify common patterns, and cleaned the data to ensure quality inputs for the model.This approach helped ensure a good variety of inputs and expected outputs, crucial for effective fine-tuning.

Additionally it was necessary verify the data's structure and integrity using Python scripts.
Finally, the data was used to calculate tokens and associated costs.

[Step 2]
Iterative process

Tell about the different datasets and finetuning jobs perfomed
and results

Notes regarding first version performace and areas to improve:
- When inputs are close to the expected answer the model gets crazy and gives responses that include parts of the prompt.
- When title is totally align the recomendation is giving a new option that it is not align with the conventions.
- When spelling mistakes the model gets crazy.
- A few details leads the model to give hypothetical situations.


[Step 3]
App development

I initially deployed a Python version of the app to a cloud environment, which allowed me to gather initial user feedback. However, unexpected billing issues made this unsustainable.

I then created a more basic version using Streamlit. While this version was well-received by users who found it useful, it lacked data storage capabilities for ongoing evaluation.

Currently, I'm rebuilding the app using React and seeking a cost-effective cloud provider for deployment. This version aims to combine user-friendliness with robust data collection for continuous improvement.

### Challenges Faced

This project wasn't without its hurdles. Some key challenges included:

- Selecting an LLM: The wide array of options across open and private sources was broad. Open-source models often required paying for computational services to run experiments, while private options were easier to manipulate but came with costs and data protection concerns. 

- Model Evaluation: Determining how to effectively evaluate and compare the results of different models is a complex task.

        - Results: Compare the performance of different models in terms of accuracy and efficiency.
        - Cost: Analyze the expenses associated with each model, including computational resources and training time.
        - Requirements: Detail the hardware and software prerequisites for running each model and for its deployment.
        - Data Privacy: Consider the privacy implications of using each model, especially regarding sensitive data.

- Deployment Costs: Finding an affordable way to deploy the app and make it available for use proved challenging.

- App Development Choices: Different options for building the app required more complex technical knowledge but offered better opportunities for improvement, such as collecting real-life interaction data for model evaluation and observation.

### Solutions and Workarounds

To address these challenges, consider including solutions like:

- LLM Selection: Conducting a thorough cost-benefit analysis of open vs. private options, considering factors like computational costs, ease of use, and data protection measures.

- Model Evaluation: Developing a structured evaluation framework, potentially including both quantitative metrics and qualitative assessments from domain experts.

- Deployment Costs: Exploring serverless architectures or containerization to optimize resource usage and reduce costs. Consider gradual rollout strategies to manage expenses.

- App Development: Opting for a modular architecture that allows for future enhancements. Implement logging and analytics from the start to facilitate data collection for ongoing model improvement.

### Results

Evaluating the fine-tuned model against the base LLM was a key part of our process. I found that while the base LLM generated outputs with accurate terminology, it struggled to consistently follow our specific style guidelines. My fine-tuned models showed improvements in adhering to our style while maintaining terminology accuracy. Additionally, the application reduced the time needed to generate suitable outputs compared to repeatedly prompting the base model.

While I don't have numerical results, I can share that after running 5 fine-tuning jobs, the latest model is performing better than the baseline. The improvements have been guided by careful evaluation of outputs and identifying specific areas of weakness, such as the model's tendency to produce nonsensical results when given misspelled inputs.

### Learnings and Insights

Some key learnings you might want to include:

- The importance of iterative development in AI projects
- The value of qualitative evaluation in addition to quantitative metrics
- The challenges and opportunities of deploying AI models in real-world scenarios
- Insights into the limitations and strengths of LLMs in specialized tasks
- The critical role of high-quality, domain-specific data in fine-tuning

### Future Improvements

Your plans align well with best practices in AI development. Consider expanding on:

- How you plan to structure your test and validation datasets
- The specific feedback mechanisms you'll implement in your React app
- Potential monitoring tools and strategies for tracking model performance
- Ideas for ensuring scalability as usage grows
- Ethical considerations and bias mitigation strategies as you collect more data

### Conclusion

In conclusion, this project has been a journey of discovery, highlighting both the potential and challenges of applying cutting-edge AI to specialized tasks. While we've made significant progress, there's still much to learn and improve.

The experience has underscored the importance of patience, iterative development, and a willingness to adapt our approach based on real-world performance. As we move forward with deployment and data collection, I'm excited to see how our fine-tuned model will continue to evolve and improve our surgical documentation process.

This project has not only enhanced our specific task but has also provided valuable insights into the practical application of AI in healthcare settings. I look forward to sharing more concrete results and insights as we gather more data from real-world usage.