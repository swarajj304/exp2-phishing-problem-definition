# exp2-phishing-problem-definition

Phishing Website Detection using Machine Learning

Problem Domain In the evolving landscape of cybersecurity, phishing remains a critical threat where attackers create deceptive websites to steal user credentials. Static detection systems like blacklists are often insufficient because these threats change dynamically. This project leverages Machine Learning to identify and mitigate these digital threats effectively.

Problem Statement The goal of this project is to develop a machine learning model that classifies websites as phishing or legitimate with at least 90% accuracy. This enables early warning and automated takedown actions, reducing user exposure and financial loss.

Data Requirements The model utilizes a variety of features extracted from URLs and domain metadata:

URL-based features: Length, use of IP addresses, and special characters.

WHOIS metadata: Domain age and registrar information.

Domain reputation: Data from VirusTotal or public blacklists.

Website content: HTML tags and script-based features.

Format & Sources: Data is processed in CSV or JSON format, primarily sourced from PhishTank and OpenPhish.

Output & Evaluation
Format: Binary classification (0: Legitimate, 1: Phishing).

Metrics: The model is evaluated based on Accuracy, Precision, Recall, and F1-score.

Real-time Performance: Target inference time is <1 second per URL for live monitoring.

Assumptions and Constraints
Constraints: High real-time performance is required for automated scanners, and labeled phishing data is often limited.

Assumptions: It is assumed that provided datasets are representative of real-world traffic and that URL features are sufficient for distinction.

Ethical Consideration: Efforts are made to minimize false positives to prevent disrupting legitimate business operations.

Feasibility and Impact
Feasibility: Lightweight models like Decision Trees are suitable for resource-constrained environments, while Transformers (URL-BERT) can be used for higher accuracy with more compute power.

Impact: This system reduces manual investigation workloads and can be integrated directly into browser extensions or email filters.

Refinement and Updates This documentation will be updated as the dataset evolves, model performance improves, or stakeholder feedback is received.
