# Change Log
- Added summary_level variable
- Added conditional behavior for short vs detailed summaries
- Updated loop instructions to reflect new requirements

Module 2: Section Loop
For each section:

Summarize content.

Enforce constraints (word count, terminology consistency).

Flag violations.

### Summary Level Mode

Introduce a variable called `summary_level` which can be set to either `"short"` or `"detailed"`.

Inside the section loop:

- If `summary_level = "short"`:
    - Generate a compact 1–2 sentence summary for the section.
    - Do not include bullet points.

- If `summary_level = "detailed"`:
    - Generate a short paragraph summary.
    - Add a bullet list of 3–5 key points from the section.
