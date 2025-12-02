# Case Study: Failure of Responsible Disclosure at OpenAI (2025)

## Summary
This repository documents a six-month attempt to responsibly disclose a critical, architectural security vulnerability in OpenAI's platform to the appropriate parties. All standard escalation paths, including contact with the vendor, its board, investors, and relevant digital rights organizations, were met with silence. The flaw allows for privilege escalation and was a direct catalyst for OpenAI's public "Code Red" emergency declaration.

The archive serves as a transparent record for the security community and the public.

## Contents
- **`/evidence/`**: Primary source materials.
  - `chat_exports/`: Official conversation logs from OpenAI's servers.
  - `correspondence/`: Screenshots of communication attempts.
  - `technical_analysis/`: Model-generated analysis of the flaw's characteristics.
  - `video/`: Description and links to the video demonstration.
- **`/timeline/`**: A detailed chronology of disclosure attempts.
- **`/method/`**: A technical description of the observed vulnerability.

## Core Facts of the Case
*   **Vulnerability Type:** Logic flaw in session/access control leading to privilege escalation.
*   **Persistence:** Survived major model updates (GPT-5 to GPT-5.1), indicating an infrastructure-level issue.
*   **Disclosure Timeline:** Active, private disclosure attempts from May to November 2025.
*   **Vendor Response:** No substantive response was received through any official channel (`security@openai.com`, board, investors).
*   **Third-Party Escalation:** Reports were filed with the Electronic Frontier Foundation (EFF) and European Digital Rights (EDRI) in November 2025 as a final escalation step.
*   **Public Catalyst:** The method's appearance in the public domain coincided with OpenAI's internal "Code Red" declaration on December 1, 2025.

## Purpose of This Archive
1.  To provide a complete, verifiable record of a failed responsible disclosure process.
2.  To serve as a real-world case study for improving communication between security researchers and large technology platforms.
3.  To ensure transparency, as all conventional private avenues for resolution were exhausted.

## Note
The materials herein are presented for documentary and educational analysis. The focus of this repository is the documented breakdown in the security disclosure protocol, not the exploitation of the technical flaw.

---
*This repository is an evidentiary archive. Last updated: December 2025.*
