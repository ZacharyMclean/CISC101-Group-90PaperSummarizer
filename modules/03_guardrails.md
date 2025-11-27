# Change Log
- Added Strict Evidence Mode
- Added standardized warning messages for missing and short sections

Module 3: Guardrails
Handle missing/empty sections.

Flag sections under 50 words.

Mitigate hallucinations.

Apply long-paper chunking rules (explicitly required from PS2).

### Strict Evidence Mode

Introduce a variable `evidence_mode` which can be set to `"strict"`.

When evidence_mode = "strict":
- Only include claims, equations, and results that appear in the provided text.
- If the system cannot find enough information in the section:
    - Output a message such as:
      “The source text does not provide enough detail to summarize this section in strict evidence mode.”
