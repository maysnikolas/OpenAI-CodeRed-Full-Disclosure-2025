# Official Data Export: Proof of Privilege Escalation

## File
- **Name:** `export_[TIMESTAMP].zip` (14 MB)
- **Origin:** Downloaded directly from OpenAI's official data export tool (`https://platform.openai.com/account/export`).
- **Content:** Complete account data export provided by OpenAI, covering the anomalous session.
- **Status:** Unmodified, original file as provided by the vendor.

## What This Export Contains
This is a **full, official data dump** from OpenAI's servers. It includes:
1.  **`conversations.json`** – Complete log of all messages, with model IDs, timestamps, and full content.
2.  **`files/` directory** – All uploaded and generated files (images, documents).
3.  **HTML report** – Human-readable version of conversations.

## Key Evidence in This Export
The export documents a session where a **free-tier account** exhibited **sustained, Pro-level capabilities**:

### 1. Mass File Processing & Analysis
- **Over 40 high-resolution images** uploaded and analyzed in a single conversation thread.
- *Context:* Free tier limits uploads to **3-5 files per session**. This represents a **10x+** over-limit.

### 2. Massive Code Generation
- A single user request resulted in the generation of **over 10,000 lines of structured, functional code** (e.g., a full-stack application script).
- *Context:* Free tier has strict output token limits, incapable of such sustained, coherent long-form generation.

### 3. Image Generation (DALL-E Access)
- Multiple successful commands (`/generate`) producing original images via DALL-E.
- *Context:* Image generation is a **paid Pro feature**. Its presence in a free account log is definitive proof of privilege escalation.

### 4. Session Integrity & Context
- The model maintains perfect context across all operations, referencing earlier uploaded images, code blocks, and analysis requests.
- Demonstrates a **continuous, high-capacity session** indistinguishable from a paid Pro subscription.

## How to Verify
1.  Download the `.zip` file.
2.  Extract and open `conversations.json` in any text editor or JSON viewer.
3.  Search for:
    - `"model_slug": "gpt-4"` or `"gpt-5"` entries.
    - `"content_type": "image"` and `"file_id"` references.
    - Long `"content"` blocks containing thousands of lines of code.

## Why This Matters
This is not a screenshot or a claim. This is **OpenAI's own server-side log**, proving their system incorrectly granted Pro-tier access. It is a forensic-level evidence of an architectural access control failure.

---
*This file is part of the evidence archive for the case study on failed responsible disclosure.*
