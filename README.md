# BUS5001 Assessment 3 ESG Cloud Evidence

This repository documents experiment evidence for BUS5001 Assessment 3.

## Q3: LLM ESG Message Triage

### Purpose
The Q3 experiment tested whether a Large Language Model could classify ESG-related operational messages into structured JSON output.

### Revised prompt
The revised prompt instructed the model to:
- return valid JSON only
- classify issue category, urgency, sentiment and follow-up need
- recommend an escalation team
- identify data sensitivity risk
- avoid inventing missing details
- list missing information

### Test messages
1. There is a water leak in Building C that has been running all morning.
2. I want to report that one of our suppliers may not meet our sustainability policy.
3. The accessible entrance near the main building has been blocked for two days.

### LLM outputs
The LLM generated JSON outputs for all three messages. The outputs included issue category, urgency, sentiment, follow-up requirement, recommended team, escalation reason, data sensitivity risk, brief summary and missing information.

### Baseline comparison
A rule-based baseline classifier was used for comparison. The baseline used keywords such as:
- water leak / running all morning
- supplier / sustainability policy
- accessible entrance / blocked / two days

The LLM and baseline were consistent for the water leak and supplier sustainability messages. The main difference was the accessibility message, where the LLM classified the issue as CRITICAL because it recognised the blocked accessible entrance as a severe accessibility barrier.

### Limitations
The LLM output may still require human review because it can over-escalate, under-escalate or assign inconsistent sensitivity ratings. HIGH and CRITICAL cases should be reviewed by a human before final operational action.

## Q4: NotebookLM Evaluation

### Purpose
The Q4 experiment evaluated Google NotebookLM as a cloud-based AI educational assistant for university coursework preparation.

### Sources uploaded
The NotebookLM notebook included:
- Assessment 3 instructions
- BUS5001 Hugging Face / LLM material
- BUS5001 Dialogflow CX workshop material

### Prompts tested
1. Summarise the key requirements of Assessment 3 for a student preparing the report. Focus on Q1, Q3 and Q4 evidence requirements.
2. What evidence is required for Q3 and Q4? Answer using only the uploaded sources and include source citations where available.
3. Create a short study guide for the ESG chatbot, LLM triage and NotebookLM evaluation parts of this assessment.

### Findings
NotebookLM was useful for source organisation, summarisation, source-grounded question answering and study guide generation. It helped identify evidence requirements and convert long assessment instructions into a practical checklist.

### Limitations
NotebookLM outputs still require checking against original sources. Students should not rely on it as a replacement for reading, critical thinking or academic writing. Privacy and copyright should also be considered before uploading documents.

## Evidence files
Screenshots for Q3 and Q4 are uploaded to this repository as supporting evidence.
