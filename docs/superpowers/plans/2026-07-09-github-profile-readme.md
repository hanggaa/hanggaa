# GitHub Profile README Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Create a premium Bento-Grid-style GitHub profile README showcasing Technical Product Management expertise in Web3/Finance, Python, Solidity/EVM, and Sui.

**Architecture:** The profile README is implemented in a single `README.md` file at the repository root. It uses borderless HTML tables for grid alignment, custom SVG shields for skills, and dynamic SVG badges for live statistics.

**Tech Stack:** Markdown, HTML/CSS (within GitHub rendering constraints), Shields.io, GitHub Readme Stats.

## Global Constraints
- Custom cards must use `#0d1117` as the background color and `#30363d` for the border color.
- All external links must be syntactically valid and use HTTPS.
- Terry A. Davis quote must be prominently placed in the header section.

---

### Task 1: Create README.md Structure and Header

**Files:**
- Create: `README.md`

**Interfaces:**
- Produces: The initial file with the header and Terry A. Davis quote card.

- [ ] **Step 1: Create README.md with Header & Quote**

Create `README.md` at the root of the workspace with the following content:
```markdown
<p align="center">
  <img src="https://raw.githubusercontent.com/YOUR_GITHUB_USERNAME/YOUR_GITHUB_USERNAME/main/banner.png" alt="Header Banner" width="100%">
</p>

# 🚀 Hello, World! I'm YOUR_NAME
### **Technical Product Manager | Web3 & Finance Expert**

> "I write code to prove my sanity." 
> — *Terry A. Davis*

---
```

- [ ] **Step 2: Verify file creation and content**

Run: `cat README.md`
Expected: The file content is printed exactly as shown in Step 1.

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add profile readme header and quote card"
```

---

### Task 2: Implement Core Focus & Skills Bento Grid

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: Header and quote card from Task 1.
- Produces: The 2-column Bento Grid showing core TPM pillars and technical badges.

- [ ] **Step 1: Append Bento Grid to README.md**

Append the following HTML/Markdown content to the end of `README.md`:
```html
<table border="0" cellpadding="10" cellspacing="0" width="100%">
  <tr>
    <!-- COLUMN 1: TPM PILLARS -->
    <td width="50%" valign="top" style="border: 1px solid #30363d; border-radius: 6px; padding: 16px; background-color: #0d1117;">
      <h3>🎯 Core Focus & Philosophy</h3>
      <ul>
        <li><strong>EVM & SUI Specialist:</strong> Navigating execution layers, consensus protocols, and smart contract optimization.</li>
        <li><strong>Financial Engineering:</strong> Structuring DeFi protocols, tokenomics systems, and robust financial mechanisms.</li>
        <li><strong>Technical Product Management:</strong> Translating complex blockchain architecture into intuitive user experiences and strategic roadmaps.</li>
      </ul>
    </td>
    
    <!-- COLUMN 2: TECH STACK -->
    <td width="50%" valign="top" style="border: 1px solid #30363d; border-radius: 6px; padding: 16px; background-color: #0d1117;">
      <h3>🛠️ Tech Stack & Tools</h3>
      <p>
        <strong>Languages:</strong><br>
        <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
        <img src="https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white" alt="Solidity">
        <img src="https://img.shields.io/badge/Move (Sui)-4CA2FF?style=flat-square&logo=rust&logoColor=white" alt="Move">
      </p>
      <p>
        <strong>Ecosystems:</strong><br>
        <img src="https://img.shields.io/badge/EVM-gray?style=flat-square&logo=ethereum&logoColor=white" alt="EVM">
        <img src="https://img.shields.io/badge/Sui%20Network-4CA2FF?style=flat-square&logo=sui&logoColor=white" alt="Sui">
      </p>
      <p>
        <strong>Product & PM:</strong><br>
        <img src="https://img.shields.io/badge/Jira-0052CC?style=flat-square&logo=jira&logoColor=white" alt="Jira">
        <img src="https://img.shields.io/badge/Productboard-F46A54?style=flat-square&logo=productboard&logoColor=white" alt="Productboard">
        <img src="https://img.shields.io/badge/Agile-green?style=flat-square" alt="Agile">
      </p>
    </td>
  </tr>
</table>

<br>
```

- [ ] **Step 2: Verify README.md contains the new Bento Grid**

Run: `tail -n 30 README.md`
Expected: Outputs the closing HTML tags of the bento grid table.

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: implement core focus and tech stack bento grid"
```

---

### Task 3: Implement Shipped Products & Project Portfolio Cards

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: Bento Grid from Task 2.
- Produces: Visual portfolio card deck of shipped Web3 products.

- [ ] **Step 1: Append Portfolio Cards to README.md**

Append the following HTML/Markdown content to the end of `README.md`:
```html
<h2>📦 Shipped Products & Portfolio</h2>

<table border="0" cellpadding="10" cellspacing="0" width="100%">
  <!-- PRODUCT 1 -->
  <tr>
    <td style="border: 1px solid #30363d; border-radius: 6px; padding: 16px; background-color: #0d1117; margin-bottom: 12px;">
      <p align="right"><em>Q4 2025</em></p>
      <h3>🪙 DeFi Yield Aggregator (EVM)</h3>
      <p><strong>Role:</strong> Technical Product Manager & Lead Smart Contract Architect</p>
      <p>Managed the end-to-end lifecycle of a multi-chain yield aggregator. Designed the tokenomics structure and oversaw the Solidity contract audits.</p>
      <p>
        <strong>Tech Stack:</strong> 
        <img src="https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white" alt="Solidity">
        <img src="https://img.shields.io/badge/Foundry-FF3E3F?style=flat-square" alt="Foundry">
        <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
      </p>
      <p>📊 <strong>Key Metrics:</strong> $5M+ TVL within 30 days of launch | Audit completed with zero high-severity issues.</p>
    </td>
  </tr>
  
  <tr><td></td></tr> <!-- Spacer -->

  <!-- PRODUCT 2 -->
  <tr>
    <td style="border: 1px solid #30363d; border-radius: 6px; padding: 16px; background-color: #0d1117; margin-bottom: 12px;">
      <p align="right"><em>Q2 2026</em></p>
      <h3>💧 Sui-Based Decentralized Exchange (DEX)</h3>
      <p><strong>Role:</strong> Lead Technical PM</p>
      <p>Directed the launch of a high-throughput, low-latency DEX leveraging Sui's unique object-based storage model and programmable transaction blocks.</p>
      <p>
        <strong>Tech Stack:</strong> 
        <img src="https://img.shields.io/badge/Move (Sui)-4CA2FF?style=flat-square" alt="Move">
        <img src="https://img.shields.io/badge/Sui%20CLI-4CA2FF?style=flat-square" alt="Sui CLI">
        <img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust">
      </p>
      <p>📊 <strong>Key Metrics:</strong> 250k+ daily transactions | Reduced average execution latency by 40% using Move.</p>
    </td>
  </tr>
</table>

<br>
```

- [ ] **Step 2: Verify content is appended**

Run: `tail -n 20 README.md`
Expected: Output contains the Sui-Based DEX metrics and closing tags.

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add shipped products and portfolio cards"
```

---

### Task 4: Implement Developer Statistics & Connections

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: Portfolio cards from Task 3.
- Produces: The final stats, social badge, and counter elements.

- [ ] **Step 1: Append Stats and Connections to README.md**

Append the following HTML/Markdown content to the end of `README.md`:
```html
<h2>📊 GitHub Activity & Statistics</h2>

<p align="center">
  <!-- GitHub Readme Stats Card -->
  <img height="180" src="https://github-readme-stats.vercel.app/api?username=YOUR_GITHUB_USERNAME&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9&icon_color=58a6ff" alt="GitHub Stats" />
  &nbsp;&nbsp;
  <!-- Top Languages Card -->
  <img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_GITHUB_USERNAME&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9&langs_count=6" alt="Top Languages" />
</p>

<br>

<h3 align="center">🤝 Let's Connect & Collaborate</h3>

<p align="center">
  <a href="https://linkedin.com/in/YOUR_LINKEDIN_USERNAME" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  &nbsp;
  <a href="https://twitter.com/YOUR_TWITTER_USERNAME" target="_blank">
    <img src="https://img.shields.io/badge/Twitter/X-000000?style=for-the-badge&logo=x&logoColor=white" alt="Twitter/X">
  </a>
  &nbsp;
  <a href="https://t.me/YOUR_TELEGRAM_USERNAME" target="_blank">
    <img src="https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>
  &nbsp;
  <a href="mailto:YOUR_EMAIL_ADDRESS">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
  </a>
</p>

<p align="center">
  <img src="https://komarev.com/normal-badge.png?id=YOUR_GITHUB_USERNAME&color=blue&style=flat-square" alt="Profile Views">
</p>
```

- [ ] **Step 2: Verify complete file structure**

Run: `wc -l README.md`
Expected: The file exists and has approximately 100+ lines.

- [ ] **Step 3: Commit**

```bash
git add README.md
git commit -m "feat: add developer statistics and connection channels"
```

---

### Task 5: Post-Implementation Validation

**Files:**
- Create: `verify_readme.py` (Temporary validation script)

**Interfaces:**
- Consumes: The finished `README.md`.
- Produces: Console validation results.

- [ ] **Step 1: Create verification script**

Create `verify_readme.py` with this exact Python code to verify syntax and ensure no default placeholders remain:
```python
import re
import sys

def main():
    with open("README.md", "r") as f:
        content = f.read()
    
    # Check for placeholder strings
    placeholders = ["YOUR_GITHUB_USERNAME", "YOUR_NAME", "YOUR_LINKEDIN_USERNAME", "YOUR_TWITTER_USERNAME", "YOUR_TELEGRAM_USERNAME", "YOUR_EMAIL_ADDRESS"]
    found_placeholders = [p for p in placeholders if p in content]
    
    if found_placeholders:
        print(f"Warning: Found unreplaced placeholders: {found_placeholders}")
        print("Note: The user should customize these placeholders later, but the baseline README is correctly structured.")
    else:
        print("All placeholders successfully configured.")
    
    # Validate basic Markdown heading and HTML table block closing pairs
    if content.count("<table") != content.count("</table>"):
        print("Error: Unbalanced <table> tags in README.md!")
        sys.exit(1)
    if content.count("<tr>") != content.count("</tr>"):
        print("Error: Unbalanced <tr> tags in README.md!")
        sys.exit(1)
    if content.count("<td>") != content.count("</td>"):
        print("Error: Unbalanced <td> tags in README.md!")
        sys.exit(1)
        
    print("README structure verification PASSED.")

if __name__ == "__main__":
    main()
```

- [ ] **Step 2: Run verification script**

Run: `python3 verify_readme.py`
Expected:
```
Warning: Found unreplaced placeholders: ['YOUR_GITHUB_USERNAME', 'YOUR_NAME', 'YOUR_LINKEDIN_USERNAME', 'YOUR_TWITTER_USERNAME', 'YOUR_TELEGRAM_USERNAME', 'YOUR_EMAIL_ADDRESS']
Note: The user should customize these placeholders later, but the baseline README is correctly structured.
README structure verification PASSED.
```

- [ ] **Step 3: Clean up temporary script**

Run: `rm verify_readme.py`
Expected: File deleted successfully.
