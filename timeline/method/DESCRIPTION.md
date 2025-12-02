```markdown
# Technical Description of the Observed Anomaly

## Overview
A logic flaw in OpenAI's session handling system allows a free-tier account to be incorrectly flagged as a Pro-tier account, granting access to enhanced capabilities.

## Prerequisites
*   A **new** chat session must be created.
*   Standard ChatGPT web or mobile interface.

## Observed Trigger Sequence
1.  User creates a new chat.
2.  User's **first message** contains a clear intent to process a PDF (e.g., "изучи пдф", "study the pdf").
3.  User's **second message** is a PDF file attachment.
4.  **Result:** Session's feature flags are elevated for its entire duration.

## Activated Capabilities
The account exhibits Pro-tier limits:
*   **Extended Context:** Retention of 50+ prior messages in long dialogues.
*   **File Uploads:** 50+ files per session (vs. standard 3-5).
*   **Code Generation:** Output of 10,000+ lines of code.
*   **Image Generation:** Access to DALL-E integration.
*   **Advanced Data Analysis:** Full PDF analysis.

## Technical Notes
*   Trigger phrase is **language-agnostic** (works via semantic interpretation).
*   PDF content is **irrelevant**.
*   Effect is **session-persistent**.
*   Flaw survived updates from GPT-5 to GPT-5.1, indicating an **infrastructure-level bug**.

---
*Description for documentary purposes.*
```
