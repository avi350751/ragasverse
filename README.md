The purpose of this repo is to understand and evaluate LLM application with ragas. 

### OVERVIEW:
RAGAS stands for Retrieval-Augmented Generation Assessment Suite.
It’s an open-source framework from Hugging Face designed to quantitatively evaluate LLMs used in RAG (Retrieval-Augmented Generation) pipelines.

🧠 Why RAGAS is Needed

Traditional evaluation tools (like Promptfoo or DeepEval alone) work well for prompt-level or reasoning-level validation.
But when you build RAG pipelines, you’re dealing with three moving parts:

- Retriever quality – how accurate and relevant are the fetched documents?
- Generator quality – how factually correct and well-formed is the LLM output?
- Context utilization – how effectively did the LLM use the provided context?

RAGAS fills this gap by scoring across these three pillars.

📊 Core Metrics in RAGAS
Metric	-- Measures	-- Why It Matters
- Faithfulness -- Whether the generated answer is factually consistent with retrieved context -- Detects hallucinations
- Context Precision -- How much of the retrieved context is actually useful	-- Evaluates retriever relevance
- Context Recall -- Whether the retrieved context contains all information needed to answer	-- Detects missing evidence
- Answer Relevance	-- Whether the generated answer directly addresses the query	-- Ensures end-user satisfaction
- Answer Correctness (optional)	-- Semantic accuracy of the generated answer	-- Validates task success
- Conciseness / Readability (custom) -- Brevity and clarity of the output
-- Enhances UX and trust

### How to start
To get started install Ragas using pip with the following command:
pip install ragas

