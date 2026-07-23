# Week 3 — AI & Generative AI Foundations for Finance

## Lineage
Turing (1930s) → AI born 1950s → shift to **ML** in the 1990s → **DL** in the 2010s
(the basis of modern AI) → **November 2022**, GenAI launches as a bridge between human
and machine. Pace toward AGI accelerating.

## The nesting (examinable distinction)
- **ML** — algorithms parse data, learn from it, make decisions from that learning.
  Best for **numeric** data.
- **DL** — a subset of ML based on neural networks; can be supervised, semi-supervised
  or unsupervised. Multiple layers progressively extract higher-level features from raw input.
- **GenAI** — a kind of DL that generates multimedia using generative models.

## What GenAI actually does today
Natural language interfaces; automates routine tasks and complex analytics; generates
tangible outcomes from abstract ideas; promotes human–human collaboration.
**Use case building presents the most significant upside.**

⚠ Quiz 1 trap: GenAI helps humans make **more informed decisions** — it does *not* make
decisions for humans, and it is *not* free of bias. Output is generated from broad-based
pre-training data that carries bias, then fine-tuned for specific tasks.

## LLMs
- Use **transformer** architectures; operate as a **statistical word prediction machine**.
- Pipeline: tokenization → pretraining → finetuning.
- **Closed-source**: black box, charged per use, commercial cloud customers, fast to market.
- **Open-source**: free to download, privately hosted, but needs specialist skills to
  fine-tune and deploy.

## Limitations and guardrails (high-yield)
Limitations: **hallucinations, biases, knowledge validity**.
Guardrails against data privacy / explainability / hallucination risk:
**RAG**, prompt engineering and chaining, value alignment, **human-in-the-loop**.

## MLOps and GenAIOps
- **MLOps** = people + processes + technology with CI/CD to operationalise ML.
  Critical: **align technical metrics with financial KPIs** in line with business goals.
- **GenAIOps** must cover: foundation model, prompt engineering, RAG operation,
  AI agent operation, evaluation, guardrailing.

## Case: Predicting Fair Value of Properties (part 1 of 2)
The property-valuation walkthrough is the course's model for **how to justify a model choice**.
The convenor explicitly said capstone technology sections must justify model selection
"kind of like how we are deciding which model to use for the prediction of house prices".
Reproduce that reasoning shape: what the data is, which candidate models, why one wins,
how the output is explained.

## Case: Ping An
A traditional Chinese insurer transformed into a global tech-driven financial services
giant. Use for: incumbent-led transformation, ecosystem strategy, tech as revenue line
rather than cost centre.

## Links from the deck
- MLOps intro: https://dev.to/andrey_s/introduction-to-mlops-managing-the-machine-learning-lifecycle-4g3j
- SSRN paper: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5540741
- GenAIOps guide: https://medium.com/google-cloud/genaiops-operationalize-generative-ai-a-practical-guide-d5bedaa59d78
- IBM AI vs ML vs DL vs NN: https://www.ibm.com/think/topics/ai-vs-machine-learning-vs-deep-learning-vs-neural-networks
