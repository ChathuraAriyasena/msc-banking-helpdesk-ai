# msc-banking-helpdesk-ai

**Multi-Task Learning and Retrieval-Augmented Generative AI for Intelligent Banking Support**

**Author:** Chathura Ariyasena  
**Programme:** MSc Computer Science – University of Staffordshire  
**Year:** 2026  

---

## Project Overview

This repository contains the implementation developed for the MSc dissertation:

*Transforming Banking Helpdesks: Leveraging Multi-Task Machine Learning and Generative AI for Intelligent Customer Service.*

The project presents an integrated AI framework designed to improve banking helpdesk operations through:

- Multi-task transformer-based ticket classification  
- Retrieval-Augmented Generation (RAG) for policy-grounded recommendations  
- Schema-controlled outputs for operational governance and consistency  

---

## Repository Structure
msc-banking-helpdesk-ai/
├── datafiles/
├── pythonfiles/
├── systemarchitecture/
├── trainedmodel/
└── README.md

---

## System Components

### Multi-Task Classification Model

Predicts:
- Intent  
- Issue Type  
- Product  
- Urgency  
- Sentiment  
- Routing Queue  

Performance:
- Macro-F1 ≈ 0.95  
- Hamming Loss ≈ 0.02  

---

### LLM Recommendation Module (RAG)

- Knowledge retrieval from external CSV-based KB  
- Embedding-based similarity search  
- Structured JSON output  

Evaluation:
- ROUGE-L Mean ≈ 0.92  
- Correctness ≈ 4.27 / 5  
- Usefulness ≈ 4.07 / 5  
- JSON validity: 100%

---

## Environment

Recommended: Google Colab (GPU)

Libraries:
- torch  
- transformers  
- pandas  
- numpy  
- scikit-learn  
- sentence-transformers  

---

## Research Contribution

- Practitioner-informed banking AI architecture  
- Multi-task learning for operational triage  
- Governance-aware generative AI design  
- Integrated evaluation across ML and LLM components  

---

## Ethics

- Fully synthetic data  
- No real customer information  
- Academic research use only  

---

## Citation

Ariyasena, C. (2026). *Transforming Banking Helpdesks: Leveraging Multi-Task Machine Learning and Generative AI for Intelligent Customer Service*. MSc Dissertation, University of Staffordshire.

---

## License

Academic use only.
For research and educational purposes.
