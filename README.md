# msc-banking-helpdesk-ai
Evidence-driven banking helpdesk AI framework combining multi-task NLP classification and retrieval-augmented generative AI for operational decision support.
Title

Banking Helpdesk AI: Multi-Task Learning + Retrieval-Augmented Generative Decision Support

⸻

1. Overview

This repository contains the implementation for the MSc dissertation:

Transforming Banking Helpdesks: Leveraging Multi-Task Machine Learning and Generative AI for Intelligent Customer Service

The system integrates:
	•	Multi-task transformer-based ticket classification
	•	Retrieval-Augmented Generation (RAG) for policy-grounded recommendations
	•	Structured, schema-controlled outputs for operational decision support

The objective is to improve triage accuracy, reduce misrouting, and support responsible AI adoption in regulated banking environments.

⸻

2. Research Context

Banking service centers process large volumes of unstructured customer requests across multiple channels. Traditional manual triage and rule-based routing often result in:
	•	Operational delays
	•	Inconsistent classification
	•	Limited adaptability to evolving customer language

This project develops an evidence-driven AI framework aligned with practitioner needs identified through a structured industry survey.

⸻

3. System Components

3.1 Multi-Task Classification Model

Predicts multiple operational attributes from ticket text:
	•	Intent
	•	Product
	•	Issue Type
	•	Urgency
	•	Sentiment
	•	Routing Queue

Evaluation
	•	Macro-F1 ≈ 0.95
	•	Hamming Loss ≈ 0.02 (clean test)
	•	Robustness tested on noisy data

⸻

3.2 Retrieval-Augmented LLM

The generative module:
	•	Retrieves relevant operational knowledge from a structured knowledge base
	•	Generates JSON-formatted action recommendations
	•	Ensures consistency and operational control

Evaluation
	•	ROUGE-L Mean ≈ 0.92
	•	Correctness Mean ≈ 4.27 / 5
	•	Usefulness Mean ≈ 4.07 / 5
	•	JSON Validity: 100%
