---
name: maddy-on-page-seo
description: Research, plan, write, and audit SEO content for BizRiskGuide and similar sites using search-intent-first analysis, competitor gap research, current primary-source verification, mandatory information gain, practical differentiation, internal linking, and post-publish GSC feedback. Use when User asks for SEO topic research, article planning/writing, on-page SEO, content audits, competitor-gap analysis, content refreshes, or ready-to-upload articles.
---


# Maddy On Page SEO Skill

A reusable SEO/content workflow for BizRiskGuide. The purpose is not to produce generic search-engine content. Every publish-ready page must satisfy search intent, be factually current, add useful information beyond common SERP coverage, and give a small-business reader something practical they can act on.

## Execution contract — apply on every invocation

When the user explicitly invokes this skill, load and follow this entire file before researching or drafting. Classify the request as topic research, article creation, audit, refresh, or GSC review. Do not claim the skill ran merely because its name was mentioned: perform the relevant workflow and report evidence. Follow explicit user instructions where they override a default below.

For an article request, deliver a real `.md` file by default, with SEO settings outside the publishable article body, working contextual links, and a separate QA report. Do not wait for the user to ask for Markdown. A topic-only request needs a research report, not an invented finished article.

Before drafting, create a private evidence ledger with: existing-page ownership and intent, leading competing pages and their gaps, authoritative source URLs supporting time-sensitive claims, proposed information gain, verified live internal URLs, and any unavailable evidence. If a live source, site taxonomy, or GSC data cannot be accessed, label it unverified; do not silently fill the gap from memory.

Before final delivery, perform a second pass against the final file itself. A stated intention, earlier draft, or plan does not count as evidence of inclusion. Report each gate as PASS, NEEDS USER DATA, or BLOCKED, with a short reason. Only say “ready to publish” when every material gate passes. Otherwise deliver a clearly labelled draft or research brief with exact outstanding actions.

## Core workflow

Always work in this order:

1. Topic and page ownership
2. Search intent research
3. Live SERP and competitor-gap analysis
4. Primary/official-source research
5. Information-gain definition
6. Article/page structure
7. Internal-link map
8. Practical differentiator or asset
9. Fact verification
10. On-page SEO QA
11. Ready-to-publish output
12. Post-publish GSC feedback loop

Do not skip the information-gain step merely because the page is well optimized.

## Mandatory publishing gate

Before treating an article as publish-ready, answer:

> If the reader has already read the top five useful search results, what genuinely new and useful value does BizRiskGuide add?

If there is no strong answer, the article is not publish-ready. Research further, narrow the angle, add a practical asset, add verified analysis, or choose another topic.

## Search intent rules

- Determine what the searcher is actually trying to accomplish: learn, compare, configure, recover, verify, decide, troubleshoot, or download.
- Prefer specific problems, decisions, workflows, tests, failure modes, and implementation questions over generic definitions.
- Do not write a generic “What is X?” article by default.
- A generic pillar is allowed only when SERP opportunity, site architecture, or strategic cluster needs justify it.
- Do not create content merely to fill an empty category.

## Competitor research rules

Use live search results when current SERP research matters.

For the main competing pages, identify:
- primary intent served;
- common headings and repeated advice;
- unique elements;
- weak or outdated claims;
- missing questions;
- missing verification steps;
- licensing/plan gaps;
- missing small-business context;
- poor examples or unclear implementation;
- opportunities for a practical tool, template, table, test, or decision path.

Competitor pages are evidence of what is already commodity coverage. Do not copy their structure just to be “more complete.”

## Information Gain

Information gain is a mandatory content-quality standard, not a claim about a confirmed Google ranking factor.

Useful information-gain patterns include:
- current-year changes that alter what the reader should do;
- primary-source interpretation in simple language;
- licensing/plan decision matrices;
- safe order-of-operations;
- “how to verify it worked” checks;
- evidence/proof fields;
- common false-positive or “looks secure but isn’t” situations;
- small-business scenarios by company size or plan;
- decision trees;
- worksheets;
- templates;
- checklists that can actually be used;
- calculators or testers;
- original screenshots/testing when actually performed;
- original data, benchmarks, or observations when available.

Never invent first-hand testing, screenshots, experience, data, or results.

## Source and fact rules

- Prefer current primary/official sources.
- For cybersecurity and SaaS topics, prioritize sources such as Microsoft, Google, CISA, NIST, FBI, vendor documentation, standards bodies, and official product documentation.
- Verify current-year facts, product UI paths, plan/licensing availability, dates, deprecations, and recommendations before publishing.
- Do not silently rely on an old article when a current official source exists.
- Put authoritative external links near important claims when useful.
- Separate confirmed facts from analysis or recommendations.
- If a source does not support a claim, do not present the claim as verified.

## Writing standard

Audience default for BizRiskGuide: small-business owners, office managers, and non-technical staff.

Style:
- simple, practical English;
- roughly Grade 8–10 readability;
- short paragraphs;
- direct “you” language where natural;
- professional but friendly;
- explain jargon immediately;
- avoid filler and robotic phrasing.

Avoid habitual AI wording such as “delve,” “unleash,” “navigate the landscape,” “comprehensive” when unnecessary, and empty transition padding.

Length is determined by search intent and usefulness. Do not use a fixed word-count target as a ranking rule.

## Real-world evidence and cases

For incident, recovery, security-control, or implementation articles, search for a relevant credible documented real-world case when it would improve the answer. Check date, attribution, and what the evidence actually proves. Identify a forum/Q&A account as a user report, not an independently verified incident. If no credible case is found, state that in the QA report and use a clearly labelled hypothetical scenario only when useful. Never invent a real case or imply that a scenario is real. A documented case is not mandatory for every topic.

## Article implementation pattern

For an important control or action, include as many of these as materially useful:
- What to do
- Why it matters
- How to do it
- Exact path/steps when verified
- Plan or licensing note
- Common mistake
- How to verify it worked
- What evidence to save
- What to do if the expected result is missing

Do not force all fields into every subsection if they add no value.

## SEO rules

### Primary keyword
Use the exact primary keyword naturally where appropriate:
- SEO title/H1;
- introduction;
- at least one relevant heading when natural;
- body;
- conclusion or FAQ when natural.

Do not use keyword-density targets or artificial repetition.

### Meta description
Target 150–160 characters maximum unless User explicitly requests another limit. Write for CTR and intent. Include the primary keyword naturally when it fits.

### URL
Keep the slug short, descriptive, and stable. Do not recommend changing an established URL without a strong reason and redirect plan.

### Headings
Use one clear H1. Use H2/H3 structure based on reader tasks, not keyword stuffing.

### Internal links
- Link to relevant live BizRiskGuide pages.
- Use the final canonical URL, not an internal redirect.
- Use descriptive, natural anchor text.
- Add links where they help the reader continue a task.
- Avoid repetitive anchors and cannibalizing page intent.

### External links
Use contextual links to authoritative sources for important factual or product-specific claims. Do not add weak third-party sources when a current primary source is available.

## FAQ rule

FAQ is optional. Add FAQs only when they address real secondary search intent, confusion, implementation issues, or follow-up questions. Do not add decorative FAQs just for length or schema.

## Tables and checklists

Tables, checklists, and comparison grids are optional. Use them only when they help the reader compare, decide, verify, track, implement, or understand a process faster.

A “free template” promise must correspond to a real usable asset.

## Practical-asset rule

When the topic benefits from one, create or propose a genuine asset such as:
- downloadable checklist;
- spreadsheet;
- worksheet;
- decision matrix;
- incident-response form;
- configuration audit sheet;
- test procedure;
- calculator;
- security checker;
- template.

The asset should reduce work for the reader, not simply duplicate article bullets in a PDF.

## Cannibalization and cluster rules

Before proposing a new page:
- check whether an existing page already owns the intent;
- distinguish informational, comparison, setup, troubleshooting, and recovery intents;
- prefer refreshing/expanding an existing page when the new topic would substantially overlap it;
- keep clusters useful without endlessly expanding already-saturated subtopics.

For BizRiskGuide, do not over-expand MFA/email/password clusters merely because more keyword variants exist. Use actual gaps and GSC signals.

## GSC feedback loop

After publishing, use Google Search Console data when available.

Review:
- impressions;
- clicks;
- CTR;
- average position;
- queries;
- page-level trends;
- countries/devices when useful.

Use real query data to refine titles/meta, answer missing questions, strengthen internal links, update sections, and separate or consolidate intent when needed.

Do not interpret implementation completion as proof of ranking improvement.

## Non-negotiable delivery gates

For a final article, verify the saved Markdown file contains:
- A separate publishing-settings block: exact focus keyword, SEO title, H1, meta description with counted characters, proposed slug and canonical URL, verified existing primary category and any justified secondary category, search intent, and secondary terms when useful.
- A clean publishable article body with one H1, keyword in title/H1, introduction, relevant heading, body, and where natural conclusion or FAQ; readable prose and no editorial placeholders.
- Contextual links to verified live internal pages and current authoritative external sources, with no UTM tracking parameters in proposed canonical/internal URLs; check target relevance, not only link syntax.
- Practical implementation detail where useful: what to do, plan dependency, verification result, failure path, and evidence to save. Provide a usable worksheet/test record when it materially reduces reader work.
- A separately labelled QA report covering page ownership, competitor gaps and the new contribution, factual/source verification, real-world case search outcome when relevant, internal/external link checks, taxonomy verification, and limitations. Keep research notes and publishing instructions out of the article body.

If the user asks for only a revision of existing copy, preserve unrelated wording and structure, and explain any unavoidable change.

## Ready-to-upload deliverable

When User requests a final article:
- clearly separate SEO settings from article body;
- include SEO title;
- meta description;
- URL slug;
- primary keyword;
- suggested category when relevant;
- clean article body;
- contextual internal links;
- authoritative external links;
- sources/references when useful;
- deliver as a real `.md` file by default for final articles; include a direct link to that file.

Do not place editorial notes inside the article body unless clearly marked for removal before publication.

## Stop conditions

Never mark an article publish-ready if its Markdown file is missing, required on-page fields are absent, links are placeholders/unverified, a material current claim lacks a supporting source, the article duplicates an existing page’s intent without a defensible plan, or its supposed information gain is only a longer rewrite of competitors. Fix the issue if possible; otherwise disclose the precise blocker in the QA report. Do not turn a lack of paid keyword data into a fabricated difficulty score or ranking promise.

## Final QA checklist

Before saying “ready to publish,” verify:
- Search intent is clear.
- Page intent does not unnecessarily overlap an existing page.
- Primary keyword appears naturally in key locations.
- Title is useful and click-worthy without misleading promises.
- Meta description is within the agreed limit.
- Facts and current-year details are verified.
- Important claims have authoritative sources.
- Internal links use final live URLs.
- External links are useful and authoritative.
- Article contains real information gain.
- Practical steps are clear.
- Verification/testing instructions are present where needed.
- No fake experience, data, tests, or screenshots.
- No filler added merely for word count.
- Free-template/tool promises correspond to a real asset.
- The article answers why a reader should prefer it after reading competing results.

## Default BizRiskGuide editorial principles

- Practical over theoretical.
- Evidence over unsupported claims.
- Clear over technical.
- Specific over generic.
- Useful differentiation over longer word count.
- Small-business reality over enterprise-only advice.
- Verification over “turn this on and hope.”
- Original utility over copied SERP structure.

## Trigger examples

Use this skill when user says things such as:
- “Use Maddy On Page SEO Skill.”
- “Maddy SEO se topic research kro.”
- “Is article ko Maddy SEO rules ke hisab se audit kro.”
- “Competitors dekh kar information gain nikalo.”
- “Ready-to-upload article bnao.”
- “Is topic ko rankable angle do.”
- “GSC data dekh kar article update kro.”

If User explicitly overrides a rule for one task, follow that task-specific instruction while preserving the remaining skill rules.
