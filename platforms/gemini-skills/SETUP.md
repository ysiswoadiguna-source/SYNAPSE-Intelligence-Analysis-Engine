# Setup: Google Gemini Skills

Gemini skills (which replace Gems) can import a `SKILL.md` file directly, so the Claude skill folder works as-is.

**Option A: upload the skill (recommended)**
1. Open the Gemini web app (gemini.google.com) or the Gemini app on Mac. Uploading skills currently isn't available on mobile.
2. Go to **Settings → Skills → Upload**.
3. Upload `synapse-intelligence-analysis/SKILL.md`, then add the five reference files from `synapse-intelligence-analysis/references/` (`analyst.md`, `scenario.md`, `techniques.md`, `biases.md`, `estimative-language.md`).
4. Save. Call it with `/` plus the skill name in the prompt box, or just describe an analysis task; Gemini can apply the skill when a prompt matches its description.

**Option B: create it manually**
1. Go to the **Skills** page and create a new skill.
2. Name: `SYNAPSE Intelligence Analysis`.
3. Description: copy the `description` line from the top of `SKILL.md`.
4. Instructions: paste [`../chatgpt-projects/INSTRUCTIONS.md`](../chatgpt-projects/INSTRUCTIONS.md). It is platform-neutral and refers to the reference files by name.
5. Add the same five reference files.

To update a skill's files, Gemini needs the whole skill uploaded again with its reference files.
