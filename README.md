# Supply-Chain-Attack--Research
🛡️ AI-Powered Traffic Monitoring for Supply Chain & MITM Attack Detection
📍 Presented as a research paper at Arizona State University – IFT 525 (AI in Cybersecurity)

📘 About the Project
This project is a practical and research-driven attempt to solve a major cybersecurity challenge faced by enterprises today—supply chain attacks and Man-in-the-Middle (MITM) threats. With increasing reliance on third-party tools and services, traditional rule-based security systems are no longer enough. Many of these attacks go unnoticed, especially when they come from “trusted” vendors or are hidden inside encrypted traffic.

To address this, I developed an AI-based web traffic monitoring system that can detect suspicious behavior in real time—even when data is encrypted.

🚀 What It Does
✅ Monitors enterprise web and network traffic for anomalies

🧠 Uses unsupervised machine learning (like Isolation Forest & DBSCAN) to detect unknown threats

🔍 Applies Explainable AI (XAI) tools like SHAP and LIME so analysts can understand why something was flagged

🔄 Incorporates Federated Learning to monitor third-party behavior without exposing sensitive data

📊 Sends real-time alerts to a custom dashboard with clear, human-readable justifications

🧠 Problem It Solves
Traditional security tools:

Are reactive and rule-based

Struggle with encrypted or obfuscated traffic

Can’t explain their alerts (black-box problem)

Don’t scale well with supply chain complexity

This system overcomes those gaps with AI-powered detection, privacy-preserving architecture, and transparency-focused design.

🧪 How It Works (Overview)
Data Ingestion: Network logs, app logs, threat intel feeds → pulled in using Apache Kafka

Preprocessing: Feature extraction + anonymization (to protect sensitive info)

Anomaly Detection: Models like Isolation Forest and DBSCAN detect patterns that deviate from normal

Explainability Layer: SHAP and LIME explain the flagged anomalies in plain English

Federated Learning: Multiple nodes learn separately and update a global model without sharing raw data

Alert System: Analyst-friendly dashboard + API integration with Splunk and Elastic tools

📊 Tech Stack
Python | Scikit-learn | TensorFlow | SHAP | LIME | Apache Kafka | AWS S3 | Wireshark | Splunk | Pandas

🔐 Key Features
Detects anomalous traffic even in encrypted communication

Preserves privacy with federated learning

Reduces false positives with intelligent clustering

Provides explainable alerts, so analysts know what’s going on

Built with a human-in-the-loop design for reliability

📈 Validation & Testing
Used simulated enterprise network traffic + anonymized real logs

Measured accuracy, precision, recall, F1 score, and latency

Analysts rated alert clarity using XAI outputs

Tested using Scikit-learn, SHAP, LIME, and TensorFlow in a cloud-simulated enterprise setup

🧩 What I Learned
How to design privacy-aware AI architectures for real-time security

The power of combining unsupervised ML + explainability

Working with Kafka pipelines, federated models, and adversarial testing

The importance of ethical AI: anonymization, fairness, transparency, and human oversight
