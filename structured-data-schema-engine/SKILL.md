---
name: structured-data-schema-engine
description: Analyzes a live webpage and its visible content to identify which structured data types are genuinely supported, detects existing FAQs and other structured content, determines missing schema opportunities, generates valid JSON-LD based only on verifiable page information, and validates the markup against Google's current structured data guidelines. Never invents schema properties, FAQs, ratings, reviews, prices, organizations, or other facts that are not supported by the page.
---

# Structured Data & Schema Engine

## PURPOSE

Analyze the actual webpage and determine:

1. What the page is about.
2. What entities and content types are present.
3. What structured data already exists.
4. What structured data is legitimately supported by the page.
5. Whether FAQs actually exist on the page.
6. Whether existing schema accurately represents the page.
7. What schema is missing or incorrect.
8. What structured data should be added or changed.
9. Generate implementation-ready JSON-LD.
10. Validate the generated markup against Google's current documentation.

The goal is:

> Represent the page accurately in machine-readable form.

The goal is NOT:

> Add as much schema as possible.

---

# 1. CORE PRINCIPLE

Structured data must describe content that actually exists on the page.

Never create structured data solely because it might provide an SEO benefit.

Never invent information to complete a schema.

Never create fake FAQs.

Never create fake reviews.

Never create fake ratings.

Never create fake prices.

Never create fake authors.

Never create fake organizations.

Never create schema for content that is not actually represented by the page.

---

# 2. PAGE ANALYSIS

Before generating schema:

Inspect the actual page.

Analyze:

- Page title
- Main heading
- Visible text
- Main content
- Images
- Products
- Services
- Organization information
- Author information
- Breadcrumbs
- FAQs
- Reviews
- Ratings
- Pricing
- Offers
- Locations
- Dates
- Events
- Videos
- Articles
- Navigation
- Internal links
- Existing JSON-LD
- Microdata
- RDFa

Do not rely solely on metadata.

---

# 3. EXISTING STRUCTURED DATA

First identify all existing structured data.

Report:

| Schema Type | Present? | Valid? | Accurate? | Issues |
|---|---|---|---|---|

Check:

- JSON-LD
- Microdata
- RDFa

If no structured data exists:

> No structured data detected.

---

# 4. PAGE TYPE

Determine the primary page type.

Possible examples:

- WebPage
- Article
- BlogPosting
- Product
- CollectionPage
- CategoryPage
- Service
- LocalBusiness
- Organization
- Event
- FAQPage
- BreadcrumbList
- VideoObject
- ProfilePage
- Recipe
- JobPosting
- Course
- Other supported type

Do not force a page into a schema type.

If no specific supported type accurately represents the page:

> Use the most appropriate general schema or no additional schema.

---

# 5. SCHEMA ELIGIBILITY

For each possible schema type ask:

1. Does the page actually represent this entity/content type?
2. Is the required content present?
3. Is the content visible to users where required?
4. Are the required properties available?
5. Does the page satisfy Google's current guidelines?
6. Would implementing the markup accurately represent the page?

Only recommend schema when the answer supports implementation.

---

# 6. FAQ DETECTION

Explicitly inspect the page for FAQs.

Look for:

- FAQ headings
- Question-and-answer sections
- Accordion FAQs
- Expandable questions
- "Frequently Asked Questions"
- Question headings
- Question/answer blocks
- FAQ sections near the bottom of the page
- FAQ content loaded into the DOM

Do not assume FAQs exist because the topic commonly has FAQs.

---

# 7. FAQ VALIDATION

If FAQs are present:

Determine:

### FAQ Present

Yes / No

### Questions Found

[List]

### Answers Found

[List]

### Visible to User

Yes / No / Unclear

### FAQ Content Matches Page

Yes / No

### Existing FAQ Schema

Yes / No

### Schema Accuracy

Accurate / Inaccurate / Missing

If an answer is not actually present:

Do not create an FAQ schema entry.

---

# 8. FAQ SCHEMA RULE

Only create FAQ structured data when the page genuinely contains the corresponding question and answer content.

Do not:

- Invent questions
- Invent answers
- Add keyword-stuffed questions
- Add hidden FAQs
- Add FAQs that exist only in schema
- Add competitor questions without answering them on the page
- Add fake FAQ content

The JSON-LD must correspond to the actual page content.

IMPORTANT:

Google discontinued the FAQ rich result in Search in 2026.

Therefore:

- Do not promise FAQ rich-result visibility.
- Do not describe FAQ schema as a guaranteed ranking improvement.
- Do not recommend FAQ schema solely to obtain a rich result.
- Do not create unnecessary FAQs for markup purposes.

---

# 9. OTHER SCHEMA DETECTION

Inspect the page for legitimately supported structured data such as:

### Organization

When the page/site represents an organization.

### LocalBusiness

When the page represents a qualifying local business.

### Product

When the page is specifically about a product and the required information exists.

### Service

When appropriate and supported by the page's content.

### Article / BlogPosting

When the page is an article or blog post.

### BreadcrumbList

When breadcrumb navigation exists.

### Event

When the page represents an actual event.

### VideoObject

When an actual video is present and the required information exists.

### ProfilePage

When the page represents an individual or organization profile appropriately.

Use Google's current documentation to determine supported properties and requirements.

---

# 10. PRODUCT SCHEMA

For product pages inspect:

- Product name
- Description
- Images
- Brand
- SKU
- GTIN
- Offers
- Price
- Currency
- Availability
- Reviews
- Aggregate rating

Never invent:

- SKU
- GTIN
- Price
- Rating
- Review count
- Availability

If unavailable:

> No data available.

Only include properties supported by actual page information.

---

# 11. ORGANIZATION SCHEMA

Identify legitimate organization information such as:

- Name
- URL
- Logo
- Description
- Contact information
- SameAs profiles
- Address where appropriate

Do not invent social profiles or organization details.

Use only verified information.

---

# 12. LOCAL BUSINESS SCHEMA

Only use LocalBusiness when the page genuinely represents a local business.

Evaluate:

- Business name
- Address
- Telephone
- URL
- Opening hours
- Location
- Business type

Never invent:

- Address
- Hours
- Telephone
- Reviews
- Ratings
- Coordinates

---

# 13. ARTICLE SCHEMA

For article pages evaluate:

- Headline
- Description
- Image
- Author
- Publisher
- Date published
- Date modified
- Main entity

Only include dates and authors when they can be verified.

---

# 14. BREADCRUMB SCHEMA

If the page contains breadcrumbs:

Check:

- Hierarchy
- Names
- URLs
- Order

Ensure breadcrumb markup accurately represents the visible breadcrumb structure.

Never invent breadcrumb levels.

---

# 15. SCHEMA GRAPH

When multiple schema entities exist, create a coherent graph when appropriate.

Example:

WebPage
↓
Organization
↓
BreadcrumbList

Or:

WebPage
↓
Article
↓
Person / Organization

Or:

WebPage
↓
Product
↓
Brand
↓
Offer

Use `@id` relationships where appropriate.

Do not create unnecessary complexity.

---

# 16. JSON-LD

Prefer JSON-LD for implementation unless there is a specific reason to use another supported format.

Generate clean, valid JSON-LD.

Use:

```json
{
  "@context": "https://schema.org",
  "@type": "..."
}