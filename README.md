# Niyukti: Evidence-Based Semantic Matching Solution 🚀

Niyukti is an evidence-based semantic matching engine designed to evaluate candidate resumes against Job Description (JD) requirements accurately while eliminating unsupported skill claims and LLM hallucinations.

---

## 🔍 Core Principle
> **"Retrieve semantically, decide deterministically, and verify with evidence."**

---

## 🛠️ Key Architectural Components
1. **Structured Extraction:** LLMs extract structured data into JSON schemas requiring mandatory source quotes[span_0](start_span)[span_0](end_span).
2. **Deterministic Rule Engine:** Plain code evaluates extracted evidence against predefined verification criteria rather than relying solely on semantic similarity[span_1](start_span)[span_1](end_span)[span_2](start_span)[span_2](end_span).
3. **Controlled Skill Taxonomy:** Manages typed relationships to differentiate terms:
   * **ALIAS:** Equivalent terms (e.g., `JS = JavaScript`)[span_3](start_span)[span_3](end_span).
   * **IMPLIES:** Directed, whitelisted relationships (e.g., `Spring Boot → Java`)[span_4](start_span)[span_4](end_span).
   * **RELATED:** Contextual connections that *cannot* independently satisfy mandatory requirements (e.g., `REST API ~ Microservices`)[span_5](start_span)[span_5](end_span).
4. **Evidence Validation:** Requires verbatim quotes and tier checks with programmatic validation[span_6](start_span)[span_6](end_span)[span_7](start_span)[span_7](end_span).

---

## 📊 Workflow & Decision Flow
* **Input:** JD + Candidate Resume[span_8](start_span)[span_8](end_span)
* **Processing:** Text parsing with offsets, structured extraction, requirement classification (eligibility vs. skill), and taxonomy normalization[span_9](start_span)[span_9](end_span).
* **Evaluation:** Rule and decision engine checks mandatory rules[span_10](start_span)[span_10](end_span).
* **Output:** Status returns either **Verified** or **Rejected + Reason Codes**, supported by complete audit logs and T&P review queues[span_11](start_span)[span_11](end_span)[span_12](start_span)[span_12](end_span).
*
