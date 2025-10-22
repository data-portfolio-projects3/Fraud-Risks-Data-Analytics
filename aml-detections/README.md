## Flagged Transactions vs. Confirmed Suspicious Activity

### Overview

In AML and fraud detection, not all flagged transactions indicate fraud or money laundering. Detection systems are designed to prioritize transactions for review, not to make definitive judgments.

**Key Principle:**

Alerts are signals for investigation. Confirmation requires analyst review and supporting evidence.

### 1. Flagged Transaction / Alert

**Definition:**
A transaction that deviates from normal patterns or matches predefined suspicious criteria (rules, thresholds, or ML models).

**Characteristics:**
*   Generated automatically by rules or anomaly detection systems.
*   Indicates potential risk, but not proof of wrongdoing.
*   Can produce false positives, especially in high-volume or cash-intensive accounts.

**Example:**

| Transaction                             | Reason for Alert                                   |
| :-------------------------------------- | :------------------------------------------------- |
| Deposit: $12,000 on a dormant account   | Exceeds historical average + regulatory threshold  |
| Multiple deposits in 7 days totaling $15,000 | Matches Velocity/Burst rule                        |

### 2. Analyst / Investigator Review

**Purpose:**
*   Validate whether the flagged transaction is truly suspicious.
*   Determine if regulatory reporting (SAR/STR) is required.

**Steps:**
*   **Review KYC/Account Information:** customer profile, account age, occupation/business type.
*   **Inspect Transactions:** timeline, amount, frequency, channels, and branches.
*   **Check Supporting Documentation:** invoices, POS receipts, contracts, digital logs.
*   **Evaluate Counterparties:** linked accounts, devices, IPs, or sanctions/PEP flags.

**Outcome:**
*   **Confirmed Suspicious:** Escalate, file SAR/STR.
*   **False Positive:** Log findings, adjust rules or thresholds to reduce recurrence.

### 3. Why Many Alerts Are Not Fraud

Detection systems favor high recall to avoid missing suspicious activity.

Legitimate transactions may trigger alerts due to:
*   Payroll, vendor payments, or legitimate business activity.
*   Large but expected deposits/withdrawals.
*   Dormant accounts suddenly activated for valid reasons.

**Key Takeaway:**
Analysts separate “signal” (true suspicious activity) from “noise” (false positives) using context, patterns, and supporting data.

### 4. Best Practices for Detection Systems

*   Include reason codes with each alert to explain why it was triggered.
*   Maintain a feedback loop: investigator dispositions are used to tune thresholds and retrain models.
*   Combine rules, risk scoring, and ML outputs for robust detection.
*   Document all investigation outcomes for audit, compliance, and regulatory review.
