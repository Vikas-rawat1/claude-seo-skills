# 🚀 Claude SEO Skills Suite

A production-grade collection of **8 specialized SEO & AI Search Skills** crafted for **Anthropic Claude** (Claude Code CLI, Claude Desktop, Claude.ai, and Claude Projects).

Transform Claude into an elite technical SEO auditor, AI search visibility strategist, Google Business Profile specialist, structured data engineer, and conversion-focused content architect.

---

## 📦 Included Skills

| Skill Name | Directory | Core Capabilities |
| :--- | :--- | :--- |
| **AI Search Intelligence** | [`ai-search-intelligence/`](./ai-search-intelligence) | Evaluates AI Overview, Perplexity, Claude & ChatGPT Search visibility, citation gaps & AEO/GEO strategy. |
| **Google Business Profile Optimizer** | [`google-business-profile-optimizer/`](./google-business-profile-optimizer) | Local 3-Pack ranking signals, GBP audits, category mapping, review strategy & prominence scoring. |
| **SEO Content Engine** | [`seo-content-engine/`](./seo-content-engine) | People-first content creation, E-E-A-T outlines, SERP gap analysis, and content brief generation. |
| **SEO Intelligence & Opportunity** | [`seo-intelligence/`](./seo-intelligence) | Root-cause traffic drop analysis, GSC/GA4 opportunity finding, and prioritized organic growth roadmaps. |
| **SEO Performance Monitor** | [`seo-performance-monitor/`](./seo-performance-monitor) | Anomaly detection, CTR decay analysis, brand vs. non-brand tracking, and campaign ROI reporting. |
| **Structured Data & Schema Engine** | [`structured-data-schema-engine/`](./structured-data-schema-engine) | Validated JSON-LD schema generation (LocalBusiness, Medical, FAQ, Article, Organization) with Google Rich Result compliance. |
| **Technical & On-Page SEO** | [`technical-onpage-seo/`](./technical-onpage-seo) | Crawlability, indexation, canonicals, robots.txt, sitemaps, internal linking structure & Core Web Vitals remediation. |
| **User Intent & Content Auditor** | [`user-intent-content-auditor/`](./user-intent-content-auditor) | Search intent fulfillment scoring, thin/generic content auditing, and conversion pathway optimization. |

---

## 🛠️ Step-by-Step Installation Guide

Choose the method matching your Claude workflow:

---

### 💻 Method 1: Installing in Claude Code (CLI)

Claude Code automatically loads custom skills placed in the `.claude/skills` directory.

#### Option A: Global Install (Available across all projects & folders)

**Windows (PowerShell):**
```powershell
# 1. Clone the repository
git clone https://github.com/Vikas-rawat1/claude-seo-skills.git

# 2. Create the global skills folder
New-Item -ItemType Directory -Force -Path "$HOME\.claude\skills"

# 3. Copy all skills to global Claude Code directory
Copy-Item -Recurse -Force .\claude-seo-skills\* -Destination "$HOME\.claude\skills\"
```

**macOS / Linux (Terminal):**
```bash
# 1. Clone the repository
git clone https://github.com/Vikas-rawat1/claude-seo-skills.git

# 2. Create the global skills directory
mkdir -p ~/.claude/skills

# 3. Copy all skills into your global Claude Code directory
cp -r claude-seo-skills/* ~/.claude/skills/
```

---

#### Option B: Project-Level Install (Specific project directory only)

If you only want these SEO skills enabled inside a specific codebase or project folder:

```bash
# In your project's root folder:
mkdir -p .claude/skills
git clone https://github.com/Vikas-rawat1/claude-seo-skills.git temp-skills
cp -r temp-skills/* .claude/skills/
rm -rf temp-skills
```

Whenever you run `claude` in your terminal, Claude Code will automatically detect and load your SEO skills!

---

### 🖥️ Method 2: Installing in Claude Desktop & Web ([claude.ai](https://claude.ai))

To install custom skills in Claude Web or Desktop, package each skill as a ZIP archive containing the skill directory and upload it directly.

#### Skill Packaging Requirement
Each custom skill must be packaged as a ZIP archive containing the skill folder with its `SKILL.md`:

```text
skill-name.zip
└── skill-name/
    └── SKILL.md
```

#### Step-by-Step Instructions:
1. **Download or clone** this repository to your computer:
   ```bash
   git clone https://github.com/Vikas-rawat1/claude-seo-skills.git
   ```
2. **Choose the skill folder** you want to install (e.g., `ai-search-intelligence`).
3. **ZIP the entire skill folder** (e.g., compress `ai-search-intelligence/` into `ai-search-intelligence.zip`).
4. **Open Claude** (Desktop App or [claude.ai](https://claude.ai)).
5. Go to **Customize** → **Skills** (or **Settings** → **Skills** depending on your interface).
6. Click **+** (or **Add**).
7. Select **Create skill** / **Upload a skill** according to the current Claude UI.
8. **Upload the ZIP** file.
   > Claude may validate or scan the uploaded skill depending on your account/workspace configuration.
9. **Enable the skill** and save.
10. **Repeat** for any other SEO skills you wish to use.

> ℹ️ **Important Note:** UI labels, button placements, and menu options may change over time as Anthropic updates the interface. Follow the current labels shown in your Claude account.
> 
> 📖 **Official Documentation:** For official details and updates on skill management, see [Anthropic Support: Use skills in Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude).

---

### 📁 Method 3: Using in Claude Projects

If you organize your workflows into Claude Projects:

1. Open your Project in **Claude** ([claude.ai/projects](https://claude.ai/projects)).
2. In the right panel, go to **Project Knowledge** or **Set Custom Instructions**.
3. Upload the `SKILL.md` file of your desired skill as Project Knowledge, or paste its markdown text directly into the Project Instructions.

---

### 📝 Method 4: Manual "Create a skill" in Claude

If you prefer copy-pasting directly into Claude's skill builder:

1. In Claude, go to **Customize** → **Skills** → **+** (or **Add**) → **Create a skill**.
2. Open the `SKILL.md` file of any skill in a text editor.
3. Fill in the fields:
   - **Name**: Copy the `name:` value from the top YAML frontmatter (e.g., `ai-search-intelligence`).
   - **Description**: Copy the `description:` value from the frontmatter.
   - **Instructions**: Copy the entire markdown content located below the frontmatter `---` separator.
4. Click **Save**.

---

## 🎯 Skill Quick Prompts & Usage Examples

### 1. 🤖 AI Search Intelligence
```text
Analyze my website [https://example.com] for AI search visibility against our competitor [https://competitor.com]. Which queries are they being cited for in AI Overviews and Perplexity that we are missing?
```

### 2. 📍 Google Business Profile Optimizer
```text
Audit our Google Business Profile for [Business Name] located in [City, State]. We offer [List of Services]. Provide a prioritized local 3-pack optimization strategy focused on relevance, distance, and prominence.
```

### 3. ✍️ SEO Content Engine
```text
Create an in-depth content brief and outline targeting 'best crm for real estate agents'. Optimize for search intent, E-E-A-T credibility, and featured snippet eligibility.
```

### 4. 🧠 SEO Intelligence & Opportunity Analyst
```text
Here is our Google Search Console export and top underperforming URLs: [paste data]. Conduct a diagnostic analysis to identify why traffic declined and give me a prioritized fix roadmap.
```

### 5. 📊 SEO Performance Monitor
```text
Review this GSC search performance dataset: [paste metrics]. Detect CTR decay anomalies, identify high-impression/low-click opportunities, and generate an executive performance report.
```

### 6. 🏷️ Structured Data & Schema Engine
```text
Generate verified JSON-LD structured data for this page: [paste URL or content]. Include LocalBusiness, WebPage, and FAQPage schemas strictly based on verifiable on-page facts.
```

### 7. 🔧 Technical & On-Page SEO Remediation
```text
Audit this page HTML and robots/canonical setup: [paste code]. Flag crawlability issues, indexation blockers, canonical discrepancies, and internal linking improvements.
```

### 8. 🎯 User Intent & Content Auditor
```text
Audit our article targeting 'how to choose dental insurance'. Does our content genuinely fulfill commercial search intent compared to top SERP competitors, or is it generic?
```

---

## 📂 Repository Directory Structure

```text
claude-seo-skills/
├── .gitignore
├── LICENSE
├── README.md
├── ai-search-intelligence/
│   └── SKILL.md
├── google-business-profile-optimizer/
│   └── SKILL.md
├── seo-content-engine/
│   └── SKILL.md
├── seo-intelligence/
│   └── SKILL.md
├── seo-performance-monitor/
│   └── SKILL.md
├── structured-data-schema-engine/
│   └── SKILL.md
├── technical-onpage-seo/
│   └── SKILL.md
└── user-intent-content-auditor/
    └── SKILL.md
```

---

## 🤝 Contributing

Contributions, additional SEO skills, and optimizations are welcome! Feel free to open an issue or submit a pull request.

---

## 📄 License

This repository is open-source and available under the [MIT License](./LICENSE).
