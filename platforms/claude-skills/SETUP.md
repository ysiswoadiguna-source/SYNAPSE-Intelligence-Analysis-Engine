# Setup: Claude Skills

**Claude app (web, desktop, mobile)**
1. Download `synapse-intelligence-analysis.skill` from the repo's Releases, or zip the `synapse-intelligence-analysis/` folder yourself (the zip must contain the folder, with `SKILL.md` inside it).
2. In Claude, open **Settings → Capabilities → Skills** and upload the file. Or open the `.skill` file in a chat and click **Save skill**.
3. Claude loads the skill automatically when a request matches, for example "analisa situasi ini", "apa maksud sebenarnya chat ini", or "buat skenario ke depan".

**Claude Code**
```bash
git clone https://github.com/ysiswoadiguna-source/SYNAPSE-Intelligence-Analysis-Engine.git
cp -r SYNAPSE-Intelligence-Analysis-Engine/synapse-intelligence-analysis ~/.claude/skills/
```

**Run the tests (Claude Code v2.1.269+)**
```bash
cd synapse-intelligence-analysis
claude plugin eval . --allow-tools Write,Edit,Bash
```
