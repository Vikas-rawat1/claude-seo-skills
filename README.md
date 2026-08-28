# 🚀 Claude SEO Skills Suite

A production-grade collection of **8 specialized SEO & AI Search Skills** tailored for **Claude** (Claude Desktop, Claude.ai, Claude Code, and Antigravity).

Turn Claude into a world-class SEO strategist, technical auditor, Google Business Profile specialist, schema architect, and AI search visibility analyst.

---

## 📦 What's Inside?

| Skill Name | Directory | Primary Focus |
| :--- | :--- | :--- |
| **AI Search Intelligence** | [`ai-search-intelligence/`](./ai-search-intelligence) | AI Overview, Perplexity, Claude & ChatGPT citation & visibility analysis |
| **Google Business Profile Optimizer** | [`google-business-profile-optimizer/`](./google-business-profile-optimizer) | Local SEO, 3-Pack ranking signals, GBP audits & strategy |
| **SEO Content Engine** | [`seo-content-engine/`](./seo-content-engine) | People-first content creation, briefs, gap analysis & SERP alignment |
| **SEO Intelligence & Opportunity** | [`seo-intelligence/`](./seo-intelligence) | Full-funnel SEO diagnosis, underperformance analysis & roadmaps |
| **SEO Performance Monitor** | [`seo-performance-monitor/`](./seo-performance-monitor) | GSC & GA4 analytics, rank tracking, anomaly detection & impact audits |
| **Structured Data & Schema Engine** | [`structured-data-schema-engine/`](./structured-data-schema-engine) | Verifiable JSON-LD schema generation & Google rich result compliance |
| **Technical & On-Page SEO** | [`technical-onpage-seo/`](./technical-onpage-seo) | Crawlability, indexability, canonicals, internal linking & page fixes |
| **User Intent & Content Auditor** | [`user-intent-content-auditor/`](./user-intent-content-auditor) | Search intent fulfillment audit, utility scoring & differentiation |

---

## 🛠️ Installation Guide

Choose your preferred way to install and use these skills:

---

### 💻 Method 1: Using with Claude Code (CLI)

You can install these skills either **globally** (available across all projects in Claude Code) or for a **specific project**.

#### Option A: Global Installation (Available in any directory)

**On Windows (PowerShell):**
```powershell
# Clone the repository
git clone https://github.com/Vikas-rawat1/claude-seo-skills.git

# Create the global skills folder if it doesn't exist
New-Item -ItemType Directory -Force -Path "$HOME\.claude\skills"

# Copy all skill folders to your global Claude Code skills directory
Copy-Item -Recurse -Force .\claude-seo-skills\* -Destination "$HOME\.claude\skills\"
```

**On macOS / Linux (Terminal):**
```bash
# Clone the repository
git clone https://github.com/Vikas-rawat1/claude-seo-skills.git

# Create the global skills directory
mkdir -p ~/.claude/skills

# Copy all skills into global Claude Code directory
cp -r claude-seo-skills/* ~/.claude/skills/
```

#### Option B: Project-Level Installation (Current workspace only)

Inside your project folder, create a `.claude/skills` directory and copy the skills:

```bash
# Inside your project root:
mkdir -p .claude/skills
cp -r /path/to/claude-seo-skills/* .claude/skills/
```

Claude Code CLI will automatically detect and load these skills during your coding and analysis sessions!

---

### 🖥️ Method 2: Upload in Claude Desktop or Web (claude.ai)

1. Open **Claude** (Desktop App or [claude.ai](https://claude.ai)).
2. Click **Customize** in the left sidebar (or go to Settings → Skills).
3. Under **Skills**, click the **Add ▾** button at the top right and select **Upload skill**.
4. **Drag and drop** the `SKILL.md` file from any skill folder, or upload a `.zip` archive containing the skill folder.
   > Claude supports:
   > - `.md` files containing YAML frontmatter (`name` and `description`).
   > - `.zip` or `.skill` files containing `SKILL.md`.
5. Claude will perform a security scan and activate the skill. Click **Save**.
6. Repeat for each skill you'd like enabled in your workspace.

---

### 📁 Method 3: Using in Claude Projects

1. Open your desired **Project** in Claude.
2. Click on **Project Knowledge** or **Custom Instructions**.
3. Upload the `SKILL.md` file or copy and paste its contents directly into the Project Instructions.

---

### 📝 Method 4: Manual "Create a skill" in Claude

1. In Claude, go to **Customize** → **Skills** → **Add ▾** → **Create a skill**.
2. Open `SKILL.md` in your text editor.
3. Fill in:
   - **Skill Name**: Name from the frontmatter (e.g., `ai-search-intelligence`).
   - **Description**: Description from the frontmatter.
   - **Instructions**: All markdown instructions below the `---` header.
4. Click **Save**.

---

## 🎯 Skill Breakdown & Example Prompts

### 1. 🤖 AI Search Intelligence (`ai-search-intelligence`)
- **Purpose**: Evaluates how well a site appears in AI search engines (Google AI Overviews, Perplexity, Claude, ChatGPT Search), identifies citation gaps, and recommends legitimate optimization opportunities.
- **Example Prompt**:
  > *"Analyze my website [https://example.com] for AI search visibility against our main competitor [https://competitor.com]. Which queries are they being cited for in AI summaries that we are missing?"*

---

### 2. 📍 Google Business Profile Optimizer (`google-business-profile-optimizer`)
- **Purpose**: Evidence-driven local SEO strategist analyzing relevance, distance, and prominence. Produces GBP audits, category recommendations, review strategies, and an HTML/UI action plan.
- **Example Prompt**:
  > *"Audit our Google Business Profile for [Business Name] in [City, State]. We offer [Services]. Provide a prioritized GBP optimization plan to improve our local 3-pack rankings."*

---

### 3. ✍️ SEO Content Engine (`seo-content-engine`)
- **Purpose**: Produces people-first, helpful content that answers search intent without fluff or generic AI phrasing. Generates briefs, outlines, and full article drafts.
- **Example Prompt**:
  > *"Create a comprehensive content brief and 1,500-word article targeting the keyword 'best crm for small businesses'. Structure it for search intent and featured snippet eligibility."*

---

### 4. 🧠 SEO Intelligence & Opportunity Analyst (`seo-intelligence`)
- **Purpose**: Holistic SEO diagnostic engine that connects technical factors, content quality, and search intent to pinpoint why pages are losing rankings and where the biggest wins lie.
- **Example Prompt**:
  > *"Our organic traffic dropped by 25% over the past 3 months on our core product pages. Here is our GSC export and top URLs: [paste data]. Conduct an SEO diagnostic and give me an action plan."*

---

### 5. 📊 SEO Performance Monitor (`seo-performance-monitor`)
- **Purpose**: Analyzes Google Search Console (GSC), Google Analytics (GA4), and ranking data to find traffic anomalies, brand vs. non-brand shifts, and ROI from SEO campaigns.
- **Example Prompt**:
  > *"Analyze this Google Search Console performance export [paste CSV or metrics]. Highlight winning queries, declining pages, click-through rate anomalies, and next steps."*

---

### 6. 🏷️ Structured Data & Schema Engine (`structured-data-schema-engine`)
- **Purpose**: Generates 100% valid, verified JSON-LD structured data markup (Article, Organization, FAQ, LocalBusiness, Product, HowTo) based strictly on actual page content.
- **Example Prompt**:
  > *"Generate complete, error-free JSON-LD schema for this page: [paste URL or page text]. Include Organization, WebPage, and FAQPage schemas properly nested."*

---

### 7. 🔧 Technical & On-Page SEO Remediation (`technical-onpage-seo`)
- **Purpose**: Technical audit tool for crawlability, indexability, canonical tags, redirect chains, XML sitemaps, robots.txt, internal linking structure, and Core Web Vitals best practices.
- **Example Prompt**:
  > *"Review our robots.txt, canonical setup, and internal link structure for our new site redesign: [paste HTML/data]. Flag any critical indexability risks."*

---

### 8. 🎯 User Intent & Content Auditor (`user-intent-content-auditor`)
- **Purpose**: Audits existing content to ensure it genuinely satisfies real search intent rather than just stuffing keywords. Scores utility, depth, and competitive differentiation.
- **Example Prompt**:
  > *"Audit our blog post [URL or paste text] targeting 'how to choose a project management software'. Does it fulfill search intent better than top 3 ranking competitors?"*

---

## 🌐 How to Publish this to Your GitHub

Follow these steps in your terminal to publish these skills to your GitHub account:

### 1. Initialize Git (if not already done)
```bash
git init
git add .
git commit -m "Initial commit: Claude SEO Skills Suite"
```

### 2. Create a Repository on GitHub
1. Go to [github.com/new](https://github.com/new).
2. Repository name: `claude-seo-skills` (or any name you prefer).
3. Set visibility to **Public**.
4. Leave "Add a README" **unchecked** (we already created one).
5. Click **Create repository**.

### 3. Link and Push to GitHub
```bash
git branch -M main
git remote add origin https://github.com/<YOUR-USERNAME>/<YOUR-REPO-NAME>.git
git push -u origin main
```

---

## 📂 Repository Structure

```text
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

## 📄 License

This project is licensed under the [MIT License](./LICENSE) - feel free to use, customize, and share!
