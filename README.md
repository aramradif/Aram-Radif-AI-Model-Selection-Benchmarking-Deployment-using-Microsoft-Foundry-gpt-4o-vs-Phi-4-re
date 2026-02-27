# Aram-Radif-AI-Choose-and-deploy-models-from-the-model-catalog-in-Microsoft-Foundry-portal

Choose and deploy models from the model catalog in Microsoft Foundry portal
GitHub

Model Selection, Benchmarking & Deployment using Microsoft Foundry (gpt-4o vs Phi-4-reasoning)
________________________________________
Project Overview
This project demonstrates how an AI Engineer:
•	Explores foundation models in the Microsoft Foundry model catalog
•	Compares models using benchmark metrics (Accuracy, Quality Index, Cost)
•	Deploys selected models to endpoints
•	Tests and evaluates performance using structured prompts
•	Optimizes outputs using prompt engineering
The project compares:
•	gpt-4o
•	Phi-4-reasoning
________________________________________
Repository Structure
ai-foundry-model-selection/
│
├── README.md
├── model-comparison.md
├── deployment-guide.md
├── prompts/
│   ├── system_prompts.txt
│   └── evaluation_prompts.txt
├── results/
│   ├── gpt4o_outputs.md
│   └── phi4_outputs.md
└── evaluation-summary.md
________________________________________
 README.md
 Problem Statement
As an AI Engineer, the goal is to:
1.	Identify the optimal foundation model for a reasoning-based generative AI application.
2.	Compare performance and cost trade-offs.
3.	Deploy models to production-ready endpoints.
4.	Evaluate real-world behavior using prompt engineering techniques.
________________________________________
 Step 1 — Explore Model Catalog
Accessed Microsoft Foundry portal:
https://ai.azure.com
Explored model details, benchmarks, and deployment options for:
•	gpt-4o
•	Phi-4-reasoning
________________________________________
 Step 2 — Model Benchmark Comparison
Metrics Evaluated
•	Accuracy
•	Quality Index
•	Cost (token-based)
•	Reasoning capability
Observations
Model	Accuracy	Quality Index	Cost	Strength
gpt-4o	High	High	Higher	Multimodal + strong general reasoning
Phi-4-reasoning	Very High	Higher	Lower	Optimized structured reasoning
Result
Phi-4-reasoning provided:
•	Better reasoning benchmark
•	Lower cost per token
•	Stronger logical problem solving
________________________________________
 Step 3 — Deployment
Deployment Type Selected
✔ Standard Deployment
✔ Global standard endpoint
✔ 50,000 Tokens Per Minute (TPM) rate limit
________________________________________
 Step 4 — Prompt Engineering Setup
System Prompt Used
You are an AI assistant that helps solve problems.
________________________________________
 Evaluation Prompts & Outputs
________________________________________
 Puzzle 1 — River Crossing Problem
Prompt
I have a fox, a chicken, and a bag of grain...
________________________________________
 gpt-4o Output
Solution Summary:
1.	Take chicken across.
2.	Return alone.
3.	Take fox across.
4.	Bring chicken back.
5.	Take grain across.
6.	Return alone.
7.	Take chicken across.
✔ Correct solution
✔ Clear explanation
________________________________________
 Phi-4-reasoning Output
Solution Summary:
Identical correct step sequence with detailed structured reasoning and intermediate state explanation.
✔ More detailed reasoning
✔ Step-by-step logical validation
________________________________________
 Puzzle 2 — Sock Problem
Prompt
I have 53 socks in my drawer...
Correct Answer: 40
________________________________________
 gpt-4o Response
Correct answer: 40
Provided reasoning using worst-case scenario logic.
________________________________________
 Phi-4-reasoning Response
Correct answer: 40
More formal worst-case breakdown:
•	Worst case: 21 blue + 17 red = 38 non-black socks
•	Add 2 more socks → guaranteed black pair
•	Total: 40
✔ Stronger structured reasoning
________________________________________
 Evaluation Summary
Criterion	gpt-4o	Phi-4-reasoning
Logical Depth	High	Very High
Explanation Clarity	High	Very Structured
Cost Efficiency	Moderate	Better
Best For	Multimodal apps	Pure reasoning apps
________________________________________
 Deployment Architecture
User → Chat App → Foundry Endpoint → Model → API Response
Each model has a unique endpoint URL.
________________________________________
 Optimization Strategies Applied
1️ Prompt Engineering
•	System persona definition
•	Explicit reasoning requests
•	Structured output formatting
2️ Reflection Prompt
Explain your reasoning.
Encourages chain-of-thought behavior.
________________________________________
 Scaling Considerations
Component	Strategy
Deployment	Standard deployment
Rate Limits	50K TPM
Monitoring	Model performance logs
Optimization	Prompt tuning before fine-tuning
Future Enhancement	RAG for domain-specific grounding
________________________________________
 Cost Consideration
Standard deployment → token-based billing
Tradeoff observed:
•	Phi-4-reasoning offered better reasoning at lower cost
•	GPT-4o offered broader flexibility (multimodal support)
________________________________________
 Cleanup
Delete resource group from Azure portal after testing to avoid charges.
________________________________________
 AI Engineer Impact
Technical Skills Demonstrated
•	Model benchmarking & comparison
•	Generative AI deployment
•	Prompt engineering
•	Performance evaluation
•	Cost optimization
•	Endpoint architecture understanding
________________________________________
 Key Learnings
•	Benchmark scores ≠ real-world performance.
•	Prompt engineering significantly improves output quality.
•	Reasoning models outperform general chat models in logic-heavy tasks.
•	Deployment strategy directly impacts cost scalability.

--

Aram Radif
