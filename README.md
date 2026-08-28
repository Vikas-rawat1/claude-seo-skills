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

## 🛠️ Step-by-Step Installation Guide

You can easily install these skills into Claude using any of the following methods.

### 🌟 Method 1: Upload Directly in Claude (Recommended)

1. Open **Claude** (Desktop App or Web at [claude.ai](https://claude.ai)).
2. Click on **Customize** (or click your profile picture/name at the bottom-left/top-right).
3. Select **Skills** from the sidebar menu.
4. Click the **Add ▾** button at the top right.
5. Click **Upload skill**.
6. Select the folder of the skill you want to add (e.g., `ai-search-intelligence` or a `.zip` archive of the folder containing `SKILL.md`).
7. Claude will automatically detect the skill name and capabilities. Click **Save**!

> 💡 **Tip:** Repeat this step for each of the 8 skill folders you want active in your Claude workspace.

---

### 📝 Method 2: Manual Copy & Paste ("Create a Skill")

If you prefer to manually configure skills inside Claude:

1. Go to **Customize** → **Skills** → **Add ▾** → **Create a skill**.
2. Open the `SKILL.md` file from the skill folder in any text editor (Notepad, VS Code, etc.).
3. **Skill Name**: Enter the name from the top frontmatter (e.g., `ai-search-intelligence`).
4. **Description**: Copy the `description` line from the top YAML frontmatter.
5. **Instructions / Prompt Content**: Copy the full text below the `---` header in `SKILL.md` and paste it into the instruction box.
6. Click **Save**.

---

### 📁 Method 3: Using in Claude Projects / Custom Instructions

If you are using **Claude Projects**:
1. Open your Project in Claude.
2. Go to **Project Knowledge** or **Custom Instructions**.
3. Upload the `SKILL.md` file or paste its contents directly into the project's system prompt instructions.

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
