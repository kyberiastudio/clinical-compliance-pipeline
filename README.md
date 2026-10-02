# M365 & Azure Clinical Governance Pipeline

This repository hosts a production-validated medical data intake and automated compliance orchestration pipeline built natively inside the **Microsoft 365 Cloud Ecosystem**. It demonstrates advanced workflow logic, role mapping configuration templates, and emergency data triage controls.

## 🛠️ System Architecture & Components
- **Intake UI Layer (Power Apps):** A custom canvas mobile interface optimized for clinic field staff to capture structured patient tracking data and incident compliance records securely.
- **Workflow Automation Engine (Power Automate):** A multi-stage backend engine that intercepts inputs, dynamically appends data matrix fields to cloud databases, and routes operational metadata.
- **Incident Response Triage (Office 365 Outlook):** Real-time automated data validation filters that immediately isolate security logs and transmit high-priority alert flags to operations when files match 'High Risk' thresholds.
- **Local Isolation Layer (Python Script):** An accompanying automated incident response script designed to parse, format, and execute a local folder lockdown during active system audit windows.

## 📂 Repository Contents
* `clinical_workflow.json` – The complete, production-exported Microsoft Power Automate backend automation schema.
* `lockdown.py` – Python automation sequence simulating emergency compliance file isolation.
* `ClinicData-Lab.xlsx` – Database scheme model tracking encounter logs and risk assessment variables.

## 📈 Compliance Logic Framework
1. **Data Ingestion:** User inputs structured telemetry through a decoupled front-end layout.
2. **Evaluation Block:** The automation fabric runs a logical split-path condition check parsing incoming `Status` inputs.
3. **Escalation Path:** If `Status == "High Risk"`, an immutable log row is saved while an immediate priority alert bypasses regular queues to signal infrastructure stakeholders.
nce-pipeline
