# msc-banking-helpdesk-ai
**Banking Helpdesk AI: Multi-Task Learning and Retrieval-Augmented Generative Decision Support**

Academic Artifact – MSc Dissertation (University of Staffordshire, 2026)
Author: Chathura Ariyasena
Programme: MSc Computer Science

⸻

Overview

This repository contains the implementation for the research project:

“Transforming Banking Helpdesks: Leveraging Multi-Task Machine Learning and Generative AI for Intelligent Customer Service.”

The project proposes an evidence-driven artificial intelligence framework designed to improve operational efficiency, accuracy, and decision quality in banking customer-support environments.

The system integrates:
	•	Multi-task transformer-based text classification for ticket understanding
	•	Retrieval-Augmented Generation (RAG) for policy-grounded action recommendations
	•	Schema-controlled outputs to support operational governance and consistency

The implementation follows a design-science research approach and aligns with practitioner requirements identified through an industry survey.

⸻

Research Motivation

Banking helpdesks process large volumes of unstructured customer inquiries across multiple digital channels. Traditional manual triage and rule-based routing often result in:
	•	Misclassification and inconsistent prioritisation
	•	Increased resolution time and operational workload
	•	Limited adaptability to evolving customer language and regulatory requirements

This project addresses these limitations by combining contextual machine learning with controlled generative AI to support intelligent, compliant decision-making.

⸻

System Architecture

1. Multi-Task Learning (MTL) Classifier

A transformer-based model predicts multiple operational attributes from ticket text:
	•	Intent
	•	Product
	•	Issue Type
	•	Urgency
	•	Sentiment
	•	Routing Queue

Performance (Test Set)
	•	Global Macro-F1 ≈ 0.95
	•	Hamming Loss ≈ 0.02
	•	Robustness evaluated using noisy data scenarios

⸻

2. Retrieval-Augmented LLM (RAG)

The generative component:
	•	Retrieves relevant operational guidance from a structured knowledge base
	•	Generates JSON-formatted action recommendations
	•	Ensures consistency, traceability, and operational control

Evaluation Results
	•	ROUGE-L Mean ≈ 0.92
	•	Correctness (1–5): Mean ≈ 4.27
	•	Usefulness (1–5): Mean ≈ 4.07
	•	JSON validity: 100%

⸻

Data

Due to privacy and regulatory constraints:
	•	No real customer data is used
	•	All datasets are synthetically generated to reflect realistic banking complaint scenarios
	•	Data is structured to support multi-task learning and operational evaluation

⸻

Environment

Recommended execution environment: Google Colab (GPU)

Required libraries:

torch
transformers
pandas
numpy
scikit-learn
matplotlib
openai (or API client)


⸻

How to Run

Step 1 – Multi-Task Model Training

Open and run:

ML_Banking_Implementation.ipynb

This notebook:
	•	Loads and preprocesses data
	•	Trains the multi-task model
	•	Evaluates classification performance

⸻

Step 2 – LLM + RAG Recommendation Module

Open and run:

LLM_Banking_Implementation.ipynb

This notebook:
	•	Loads the knowledge base
	•	Generates embeddings
	•	Retrieves relevant policy context
	•	Produces structured action recommendations

⸻

Research Contribution

This work provides:
	•	A practitioner-informed AI architecture for banking service operations
	•	Empirical evidence for multi-task learning in operational triage
	•	A controlled RAG-based generative framework for regulated environments
	•	Integrated evaluation using quantitative metrics and expert-aligned assessment
	•	A scalable approach to responsible AI adoption in financial customer service

⸻

Ethical Considerations
	•	No real customer or institutional data used
	•	Synthetic and publicly inspired datasets only
	•	No integration with live banking systems
	•	Designed in accordance with responsible AI and research ethics principles

⸻

Author

Chathura Ariyasena
MSc Computer Science
University of Staffordshire
United Kingdom
2026

⸻

Citation

If referencing this work:

Ariyasena, C. (2026). Transforming Banking Helpdesks: Leveraging Multi-Task Machine Learning and Generative AI for Intelligent Customer Service. MSc Dissertation, University of Staffordshire.
