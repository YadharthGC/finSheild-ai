# FinShield AI — Intelligent Credit Risk & Fraud Detection Platform

A production-grade AI platform that combines real-time fraud detection 
and LLM-powered credit risk assessment built to mirror Capital One's IFX team stack.

---

## Week 1 — Data Layer

### Day 1 — Synthetic Transaction Data Generator

**What I built:**
A Python script that generates realistic credit card transaction data from scratch.

**What the data looks like:**
- 1000 transactions with 6 features each
- 1.5% fraud rate (mirrors real-world fraud rates)
- Fraud transactions have distinct patterns vs legitimate ones

**Features generated:**
- `transaction_id` — unique ID per transaction
- `amount` — normal distribution around $200 for legitimate, $800 for fraud
- `merchant_category` — electronics, grocery, restaurant, travel
- `country` — US/UK/IND/BRA for legitimate, NG/RO/UA for fraud
- `hour_of_day` — business hours for legitimate, 0–4am for fraud
- `is_fraud` — 0 or 1

**Key concepts learned:**
- Class imbalance — why accuracy is a useless metric for fraud detection
- Precision vs Recall — Capital One prioritizes recall over precision
- Why fraud transactions need different feature distributions to be learnable

**Files:**
- `transactions.csv` — 1000 synthetic transactions

---

## Tech Stack
- Python, CSV, Random (Day 1)
- More coming Week 1 Day 2–7...
