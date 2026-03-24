# Explainable Anomaly Detection in Information Systems: State of the Art and Application to Timekeeping and Payroll Systems

**Author:** EL ARGOUBI El Mehdi  
*Engineering School of the Littoral Côte d’Opale (EILCO), University of the Littoral Côte d’Opale (ULCO), Calais, France*

---

## Abstract
Timekeeping and payroll information systems play a vital role in organizations, as they process sensitive data with a direct impact on employees, regulatory compliance, and financial governance. The reliability of this data is therefore a major challenge for management processes. However, these systems are exposed to anomalies resulting from entry errors, inconsistencies, or fraudulent behavior, which can affect data quality and user trust. Traditional control mechanisms reach their limits in the face of increasing data complexity. In this context, the literature is moving towards automated explainable anomaly detection approaches. In sensitive areas like payroll, detection alone is insufficient and must be supplemented by explainability mechanisms. This study proposes a state-of-the-art review of explainable anomaly detection approaches applied to timekeeping and payroll systems.

**Keywords:** Information Systems, Fraud Detection, Explainable AI (XAI), Anomaly Detection, ERP, Human Resource Systems.

---

## 1. Anomaly Detection: Concepts and Challenges

### 1.1 Definition of Anomalies
In management systems, an anomaly corresponds to a deviation from the expected operation, as defined by historical data, business rules, or organizational processes—this normality being dependent on the application context. It is essential to distinguish the anomaly from other related notions: **error** (unintentional, related to entry or processing), **inconsistency** (contradiction between information or rules), and **fraud** (intentional violation for gain). An anomaly serves as a generic warning signal, aiming to draw human attention to situations requiring in-depth analysis.

### 1.2 Typologies of Anomalies
The literature distinguishes three main categories of anomalies:
- **Statistical Anomalies**: Atypical numerical values compared to a reference behavior (common in transactional and temporal data).
- **Behavioral Anomalies**: Unusual action patterns or user profiles, detectable through temporal analysis or peer comparison.
- **Logical Anomalies**: Violations of rules or business constraints, even when individual values appear consistent.

---

## 2. Anomaly Detection Approaches in Management Systems

### 2.1 Rule-Based Approaches
The historical first level of control, relying on the explicit formalization of business rules from regulatory or organizational frameworks. While simple, transparent, and easy to audit, they are poorly adapted to evolving behaviors and struggle to detect new or subtle anomalies.

### 2.2 Statistical and Exploratory Approaches
These detect anomalies by identifying atypical values through data distribution analysis. Particularly suited for tabular and numerical data in payroll systems, they identify significant deviations in hours worked or remuneration amounts. However, they often provide limited explanations, simply indicating that a value is atypical.

### 2.3 Advanced Approaches Applied to ERP
Increasingly, ERP anomaly detection relies on analyzing transactional logs and business process execution traces. These model event sequences and user behaviors to detect process anomalies rather than just outliers. While they offer better detection capabilities, they reinforce the need for explainability to link alerts back to process steps or business rules.

---

## 3. Explainability of Anomalies

### 3.1 Why Explain an Anomaly?
In critical management systems, an unexplained alert is difficult to exploit. Explainability transforms automatic detection into **actionable information** by identifying the factors that led to the anomaly. It also ensures traceability and auditability, essential for compliance in payroll and HR.

### 3.2 Types of Explanations
- **Post-hoc Approaches**: Methods like **LIME** (local approximation) and **SHAP** (Shapley values) are used to explain complex models by identifying influential variables.
- **Intrinsically Explainable Models**: Models based on rules or logical constraints that integrate explainability directly into the detection process.
- **Local vs. Global**: Local explanations (centered on a specific alert) are preferred in payroll systems where each anomaly must be analyzed individually.

---

## 4. Application to Timekeeping and Payroll Systems
Payroll systems rely on structured, tabular, and temporal data from HR and ERP systems. Anomalies can be statistical (high volume of hours) or behavioral (recurrent overtime). Logical anomalies, such as conflicts between overtime and contracts, are particularly critical. Explainable approaches reduce investigation time by linking anomalies to specific rules or variables, fostering user acceptance and regulatory compliance.

---

## 5. Discussion and Research Perspectives
Automated anomaly detection is a key lever for controlling management information systems. However, in sensitive contexts like payroll, detection alone is insufficient. Explainability is central to building user trust and supporting human decision-making. Future research will focus on improving explainability for mixed and temporal data, deeper integration of business rules, and fully auditable detection frameworks.

---

## 6. Conclusion
This bibliographic research presented a state-of-the-art review of explainable anomaly detection in information systems. While traditional and statistical approaches are useful, they struggle with increasing data complexity. Advanced ERP-applied approaches offer better detection but require explainability to ensure understanding, trust, and auditability in sensitive contexts like payroll.

---

## 7. References
1. **Wang, N., Zhang, X., Li, S., & Gao, X. (2025)**. Applications of artificial intelligence in enterprise human resource management. *Information Resources Management Journal*, 38(1), 1–19.
2. **Saha, S., & Goel, P. (2023)**. Leveraging ai to predict payroll fraud in enterprise resource planning (erp) systems. *International Journal of Information Management*, 73.
3. **Ravichandran, S., Krishnan, R., & Balaji, M**. Ai-powered payroll fraud detection: Enhancing financial security in hr systems. *Journal of Financial Crime*, 31(2).
4. **Islam, S. R., Eberle, W., Ghafoor, S. K., & Ahmed, M. (2021)**. Explainable artificial intelligence approaches: A survey. *IEEE Access*, 9, 124000–124035.
5. **Schmid, S., Assent, I., & Müller, E. (2023)**. Anomaly explanation: A survey. *ACM Computing Surveys*, 55(7), 1–38.
6. **Li, Z., Zhu, J., & van Leeuwen, M. (2023)**. A survey on explainable anomaly detection. *ACM Transactions on Knowledge Discovery from Data*, 17(3), 1–41.
7. **Jamithireddy, N. H. (2023)**. Driven anomaly detection and root cause analysis in sap erp using hybrid neural-symbolic systems. *Procedia Computer Science*, 219, 481–490.
8. **Milojković, N., Kljajić, M., & Dakić, B. (2025)**. Z-score and validoai: An explainable ai framework for payroll analytics with statistical anomaly detection in smes. *Expert Systems with Applications*, 238.
9. **Kwon, Y., Moon, D., Oh, Y., & Yoon, H. (2025)**. Logicqa: Logical anomaly detection with vision-language model generated questions. *Pattern Recognition*, 151.
10. **Kumar, N., Sharma, V., & Sharma, A. (2025)**. Artificial intelligence in fraud prevention: Techniques, applications, challenges and opportunities. *Journal of Big Data*, 12(4).
11. **Tritscher, J., Keller, F., & Müller, E. (2023)**. Feature relevance xai in anomaly detection: Reviewing approaches and challenges. *Data Mining and Knowledge Discovery*, 37, 1–35.
12. **Mohammad, A. J. (2021)**. Ai-augmented time theft detection system. *International Journal of Advanced Computer Science and Applications*, 12(6), 98–107.
13. **Yepmo, V., Ndiaye, L., & Dipanda, A. (2022)**. Anomaly explanation: A review. *Artificial Intelligence Review*, 55, 4567–4602.
14. **Botana, I. L., Pau, R., & Domingo-Ferrer, J. (2022)**. Explanation method for anomaly detection on mixed numerical and categorical spaces. *Information Sciences*, 585, 1–18.
15. **Gummadi, A. N., Kumar, P., & Patra, S. R. (2024)**. Xai-iot: An explainable ai framework for enhancing anomaly detection in iot systems. *Future Generation Computer Science*, 148, 178–191.
16. **Bello, O. A., & Olufemi, K. (2024)**. Artificial intelligence in fraud prevention: Applications, challenges and future directions. *Journal of Information Security and Applications*, 76.
