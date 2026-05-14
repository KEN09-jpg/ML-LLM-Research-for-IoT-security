# ML-LLM-Research-for-IoT-security
HybridShield — IoT Malware Detection Framework
A proposed two-stage hybrid framework for IoT malware detection and vulnerability assessment that combines traditional Machine Learning with Large Language Models.
Stage 1 uses a lightweight Random Forest or XGBoost classifier to rapidly screen high-volume network traffic, filtering out benign packets and flagging suspicious cases. Stage 2 deploys a quantized fine-tuned BERT model to perform deep contextual analysis on flagged traffic, detecting novel malware and zero-day exploits that traditional ML cannot catch. A RAG-powered vulnerability assessment module cross-references detected threats against live CVE data and generates human-readable security reports.
Built with
Python · Scikit-learn · HuggingFace Transformers · BitsAndBytes · LangChain · FAISS · MQTT
Datasets
UNSW-NB15 · IoT-23 · N-BaIoT · TON-IoT
Key results from supporting literature

BERT-based models achieve up to 98.2% accuracy on IoT security tasks
8-bit quantization reduces model size by 63% with only 0.02% accuracy drop
RAG integration reduces threat assessment response time by 17%
Framework reduces LLM invocations by 70-80% through ML pre-filtering

Based on
Jamshidi et al., "The Role of Large Language Models in IoT Security: A Systematic Review of Advances, Challenges, and Opportunities," Internet of Things, vol. 34, p. 101735, 2025.
