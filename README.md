# 5G Signaling Analysis Agent Workflow

A multi-agent intelligent system designed to 5G Signaling Analysis Agent, from raw PCAP parsing to structured root cause analysis and actionable report generation.


## 1. Frontend Demo Interface
The interactive dashboard provides end-to-end visualization of the analysis workflow, from task submission to final report display.
![agent_demo_ui.png](https://github.com/lichong-007/5G-Signaling-Analysis-Agent_workflow/blob/main/assets/agent_demo_ui.png)

---

## 2. 5G Signaling Procedure Mapping
A structured knowledge base that maps 3GPP-defined procedures, message types, and error codes to business contexts, enabling precise event correlation.
![5g_procedure_mapping](https://github.com/lichong-007/5G-Signaling-Analysis-Agent_workflow/blob/main/assets/5g_procedure_mapping.png)

---

## 3. Raw Signaling Capture Parsing
Directly processes Wireshark PCAP traces to timestamps, and failure causes, with full NAS/S1AP protocol decoding support.
![wireshark_capture](https://github.com/lichong-007/5G-Signaling-Analysis-Agent_workflow/blob/main/assets/wireshark_capture.png)

---

## 4. Structured Data 
## 4. Structured Raw Data for RAG
Standardized structured raw data prepared for the RAG retrieval system, before any text conversion or processing.
![original structured data](https://github.com/lichong-007/5G-Signaling-Analysis-Agent_workflow/blob/main/assets/original structured data.png)

---

## 5. Backend API Response
The analysis results are exposed via a API, delivering machine-readable reports with clear root cause analysis and step-by-step troubleshooting recommendations.
![backend_api_response ](https://github.com/lichong-007/5G-Signaling-Analysis-Agent_workflow/blob/main/assets/backend_api_response .png)

---

## Core Capabilities
- **Protocol-Aware Parsing**: Decodes 5G NAS/S1AP signaling and maps events to business procedures
- **Multi-Agent Reasoning**: Uses task decomposition to handle complex, multi-step failure scenarios
- **Root Cause Correlation**: Identifies causal relationships between events
- **Actionable Recommendations**: Generates telecom-standard troubleshooting steps aligned with 3GPP specifications

## Tech Stack
- Orchestration: LangGraph
- LLM Reasoning: Domain-adapted large language model
- Signaling Parsing: Custom 3GPP protocol decoder
- Backend: FastAPI, Python
- Data Processing: Pandas, structured rule engine
- Frontend: Streamlit interactive dashboard
