# PhishGuard AI

PhishGuard AI is an end-to-end phishing detection and security analysis platform designed to identify potentially malicious emails and messages using natural language processing, machine learning, URL analysis, and agent-based investigation workflows.

The project focuses on building a practical ML engineering pipeline covering data preprocessing, model training, evaluation, API-based inference, and deployment.

## Problem Statement

Phishing attacks frequently rely on social engineering techniques such as impersonation, urgency, credential requests, malicious links, and deceptive messaging.

Traditional rule-based filters can struggle with continuously changing attack patterns. PhishGuard AI aims to combine machine learning with structured security analysis to identify phishing indicators and provide an interpretable risk assessment.

## Objectives

The project aims to:

- Classify emails and messages as legitimate, suspicious, or phishing.
- Extract and analyze phishing-related indicators from message content.
- Identify potentially suspicious URLs and domains.
- Develop and compare traditional NLP and transformer-based models.
- Provide an interpretable risk score and classification explanation.
- Expose the trained model through a REST API.
- Develop an agent-based workflow for structured security investigation.
- Evaluate the system using standard machine learning metrics and inference latency.

## System Overview

```text
Email / Message
       |
       v
Input Processing
       |
       +-------------------+
       |                   |
       v                   v
Email NLP Analysis    URL Analysis
       |                   |
       +---------+---------+
                 |
                 v
          Risk Assessment
                 |
                 v
       Phishing Classification
                 |
                 v
       Security Investigation
                 |
                 v
      Explanation & Recommendation
                 |
                 v
          FastAPI Service
                 |
                 v
        Web-based Dashboard
