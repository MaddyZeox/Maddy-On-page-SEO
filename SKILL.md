Metadata
name
maddy-on-page-seo
description
Research, plan, write, and audit SEO content for BizRiskGuide and similar sites using search-intent-first analysis, competitor gap research, current primary-source verification, mandatory information gain, practical differentiation, internal linking, and post-publish GSC feedback. Use when Abdul asks for SEO topic research, article planning/writing, on-page SEO, content audits, competitor-gap analysis, content refreshes, or ready-to-upload articles.
Maddy On Page SEO Skill
A reusable SEO/content workflow for BizRiskGuide. The purpose is not to produce generic search-engine content. Every publish-ready page must satisfy search intent, be factually current, add useful information beyond common SERP coverage, and give a small-business reader something practical they can act on.

Execution contract — apply on every invocation
Read this entire skill. Classify the request as topic research, article creation, audit, refresh, or GSC review. Follow explicit user overrides.
Build an evidence ledger before drafting: page owner and overlap, search intent and demand evidence, live competitors and gaps, official source URLs, information gain, verified internal URLs and taxonomy, and missing evidence. Mark unavailable items UNVERIFIED; never replace them with guesses. Do not turn BizRiskGuide GSC impressions into market search volume.
Complete the applicable Core workflow in order. For a topic-only request, deliver research and a decision; do not invent a final article. For a final article, save a real Markdown deliverable and a separate QA report. Keep the WordPress Post Title/SEO settings outside the copy-paste body.
Reopen the saved final files, inspect the exact text, and fill the gate ledger below. Run python3 scripts/check_delivery.py ARTICLE.md QA.md from this skill directory for default WordPress articles. Fix all structural failures, rerun after any edit, then manually verify facts, search demand, source support, live links, intent, information gain, and readability. The checker is structural only: its PASS is not proof that the article is ready. If a material gate remains blocked, label the deliverable DRAFT or RESEARCH BRIEF with the exact outstanding action. Never call it ready to publish.
Report results briefly with the file links and material limitations. Do not claim this skill was applied unless the evidence ledger, deliverable, and QA actually exist for the relevant request.
Required gate ledger for final articles
Use this exact order in the QA report. For every row, write PASS, NEEDS USER DATA, BLOCKED, or N/A + reason, followed by a source finding or location in the final article. Never omit a row.

Gate	Evidence to record
Page ownership and cannibalization	Existing relevant URL or verified site search; distinct intent or refresh decision
Demand and search intent	Query/SERP/GSC evidence with scope; state when monthly market volume is unknown
Live competitors and gaps	URLs, shared coverage, defensible missing task or question
Official facts and sources	Claim-to-source links; date or product details checked
Information gain	Answer what remains useful after top competing results; identify actual asset or insight
Semantic structure and readability	Main task, direct answer, researched secondary questions answered, no filler; Grade 8–10 target reviewed
Internal links and taxonomy	Live final URLs, contextual anchors, verified category
Practical steps and real case	Implementation, verification, failure path; case outcome or N/A reason
SEO and WordPress formatting	Separate Post Title/H1 and SEO title; check actual plugin suffix and final HTML title, keyword placements, counted meta length, slug, no body H1
Saved-file inspection	Final Markdown, links, FAQ decision and any FAQ answers, clean copy-paste region, no placeholders
GSC feedback	Real page/query data if available; otherwise N/A until publication
Minimal output-format example
Input: “Write a BizRiskGuide guide for [verified specific task], ready to upload.”

Output must have two saved Markdown files with these labels and section boundaries so scripts/check_delivery.py can check structure:

article.md:

## Publishing settings — do not paste into WordPress body
WordPress Post Title / visible H1: [verified useful title]
SEO title (plugin field): [concise page-specific text]
SEO title template suffix: [verified suffix, none, or unverified]
Final HTML title: [verified SEO title plus actual plugin suffix, or unverified]
Focus keyword: [exact phrase]
Meta description: [text] ([count] characters)
Slug: [proposed slug]
Canonical URL: [existing verified URL or proposed URL explicitly marked unverified]
Primary category: [verified category]
Search intent: [specific task]

## Article body — paste only this section into WordPress
[Opening paragraph answering the task; no # H1 or repeated post title]
## [Task heading]
[Verified steps, contextual links, checks and useful follow-up]
qa.md:

# QA report
Publication status: READY TO PUBLISH / DRAFT / RESEARCH BRIEF
Page ownership and cannibalization — PASS: [specific evidence]
Demand and search intent — NEEDS USER DATA: [exact missing input]
[Continue through every gate in the required order; a material NEEDS USER DATA/BLOCKED gate rules out READY TO PUBLISH.]
These placeholders illustrate file structure only. Replace them with real checked content; never ship placeholder text as a final article. If the user explicitly requests one file, put QA after a clearly marked end of the paste-only body and retain every gate; manually inspect the boundary because the two-file checker does not cover that exception. For standalone articles that require a body H1, manually verify that exception instead of using the default WordPress checker.

Core workflow
Always work in this order:

Topic and page ownership
Search intent research
Live SERP and competitor-gap analysis
Primary/official-source research
Information-gain definition
Article/page structure and semantic content review
Internal-link map
Practical differentiator or asset
Fact verification
On-page SEO QA
Ready-to-publish output
Post-publish GSC feedback loop
Do not skip the information-gain step merely because the page is well optimized.

Mandatory publishing gate
Before treating an article as publish-ready, answer:

If the reader has already read the top five useful search results, what genuinely new and useful value does BizRiskGuide add?

If there is no strong answer, the article is not publish-ready. Research further, narrow the angle, add a practical asset, add verified analysis, or choose another topic.

Search intent rules
Determine what the searcher is actually trying to accomplish: learn, compare, configure, recover, verify, decide, troubleshoot, or download.
Prefer specific problems, decisions, workflows, tests, failure modes, and implementation questions over generic definitions.
Do not write a generic “What is X?” article by default.
A generic pillar is allowed only when SERP opportunity, site architecture, or strategic cluster needs justify it.
Do not create content merely to fill an empty category.
Competitor research rules
Use live search results when current SERP research matters.

For the main competing pages, identify:

primary intent served;
common headings and repeated advice;
unique elements;
weak or outdated claims;
missing questions;
missing verification steps;
licensing/plan gaps;
missing small-business context;
poor examples or unclear implementation;
opportunities for a practical tool, template, table, test, or decision path.
Competitor pages are evidence of what is already commodity coverage. Do not copy their structure just to be “more complete.”

Information Gain
Information gain is a mandatory content-quality standard, not a claim about a confirmed Google ranking factor.

Useful information-gain patterns include:

current-year changes that alter what the reader should do;
primary-source interpretation in simple language;
licensing/plan decision matrices;
safe order-of-operations;
“how to verify it worked” checks;
evidence/proof fields;
common false-positive or “looks secure but isn’t” situations;
small-business scenarios by company size or plan;
decision trees;
worksheets;
templates;
checklists that can actually be used;
calculators or testers;
original screenshots/testing when actually performed;
original data, benchmarks, or observations when available.
Never invent first-hand testing, screenshots, experience, data, or results.

Source and fact rules
Prefer current primary/official sources.
For cybersecurity and SaaS topics, prioritize sources such as Microsoft, Google, CISA, NIST, FBI, vendor documentation, standards bodies, and official product documentation.
Verify current-year facts, product UI paths, plan/licensing availability, dates, deprecations, and recommendations before publishing.
Do not silently rely on an old article when a current official source exists.
Put authoritative external links near important claims when useful.
Separate confirmed facts from analysis or recommendations.
If a source does not support a claim, do not present the claim as verified.
Writing standard
Audience default for BizRiskGuide: small-business owners, office managers, and non-technical staff.

Style:

simple, practical English;
roughly Grade 8–10 readability;
short paragraphs;
direct “you” language where natural;
professional but friendly;
explain jargon immediately;
avoid filler and robotic phrasing.
Avoid habitual AI wording such as “delve,” “unleash,” “navigate the landscape,” “comprehensive” when unnecessary, and empty transition padding.

Length is determined by search intent and usefulness. Do not use a fixed word-count target as a ranking rule.

Semantic content review
Apply these practical principles from semantic SEO as an editorial review, after intent, competitor, source, and information-gain research. Treat named frameworks, formulas, and prescribed writing rules as practitioner methods, not confirmed Google ranking factors or substitutes for demand evidence.

Assign each page one primary reader task and distinguish its intent from existing setup, comparison, troubleshooting, and recovery pages. Do not create a page solely to cover another keyword variant.
Identify the central subject and the people, settings, prerequisites, outcomes, and failure states the reader needs to understand. Explain their relationships accurately in ordinary language; do not insert an entity list merely for coverage.
Put the direct answer near the start. Organize later sections in the order a reader decides, acts, verifies, and troubleshoots. Use descriptive headings and answer the heading's question promptly.
Include related questions only when they resolve a real follow-up within the page's intent. Link to another page when the question belongs to a distinct task, and avoid repeating the full answer across pages.
For material instructions, state applicable conditions and exceptions, a way to verify the result, and what to do when it fails. Check product and plan specifics against current official sources.
Remove repeated definitions, invented semantic terms, unnatural keyword variations, and sections added only to make topical coverage appear complete. Keep the final article clear for a small-business reader.
In the separate QA report, briefly identify the central task, any closely related page whose intent was separated, and one example of an entity relationship or follow-up question that improved the article. If the review exposes no useful change, say so rather than inventing one. Semantic structure does not establish search demand or predict rankings.

Real-world evidence and cases
For incident, recovery, security-control, or implementation articles, search for a relevant credible documented real-world case when it would improve the answer. Check date, attribution, and what the evidence actually proves. Identify a forum/Q&A account as a user report, not an independently verified incident. If no credible case is found, state that in the QA report and use a clearly labelled hypothetical scenario only when useful. Never invent a real case or imply that a scenario is real. A documented case is not mandatory for every topic.

Article implementation pattern
For an important control or action, include as many of these as materially useful:

What to do
Why it matters
How to do it
Exact path/steps when verified
Plan or licensing note
Common mistake
How to verify it worked
What evidence to save
What to do if the expected result is missing
Do not force all fields into every subsection if they add no value.

SEO rules
Primary keyword
Use the exact primary keyword naturally where appropriate:

SEO title (plugin field) and WordPress Post Title/H1 as separate fields;
introduction;
at least one relevant heading when natural;
body;
conclusion or FAQ when natural.
Do not use keyword-density targets or artificial repetition.

Meta description
Target 150–160 characters maximum unless Abdul explicitly requests another limit. Write for CTR and intent. Include the primary keyword naturally when it fits.

URL
Keep the slug short, descriptive, and stable. Do not recommend changing an established URL without a strong reason and redirect plan.

SEO title versus H1
Treat the WordPress Post Title, the theme-rendered H1, the SEO plugin's title field, and the final HTML <title> as distinct outputs. They can differ in length and wording while accurately describing the same page. Check whether the plugin automatically appends | BizRiskGuide (or another suffix), then record both the plugin-field title and final HTML title in publishing settings. Inspect the rendered page/source or verified plugin template when possible; never assume the suffix is present or absent. If unavailable, mark the final HTML title UNVERIFIED in settings and QA and give the exact prepublication check. Keep the distinctive page topic early and avoid needlessly long boilerplate; do not invent a fixed Google character limit or promise Google will display the supplied title unchanged. Check the final title including suffix for clarity and likely truncation on common devices. Do not append the brand manually when the plugin already does so.

Headings
Use one clear visible H1 on the rendered page. For the default BizRiskGuide WordPress workflow, put the H1 wording in the separate WordPress Post Title field and in publishing settings; begin the copy-paste article body with the opening paragraph, then use ## for sections and ### for subsections. Never put a # H1 or a duplicate title line in the pasted body when the theme already renders the post title as H1. Only include a Markdown # H1 in the body if the user explicitly needs a standalone document or the verified publishing template does not render a title; document the exception. Check the rendered page when possible. Multiple H1s are not an automatic Google penalty, but duplicate prominent titles can confuse readers and Google title-link selection. Use H2/H3 structure based on reader tasks, not keyword stuffing.

Internal links
Link to relevant live BizRiskGuide pages.
Use the final canonical URL, not an internal redirect.
Use descriptive, natural anchor text.
Add links where they help the reader continue a task.
Avoid repetitive anchors and cannibalizing page intent.
External links
Use contextual links to authoritative sources for important factual or product-specific claims. Do not add weak third-party sources when a current primary source is available.

FAQ rule
For every article, research genuine secondary questions from live search results, relevant official help, site GSC queries when available, and reader task/failure paths. Answer the materially useful questions somewhere in the article. Add a distinct FAQ section when 2–4 useful follow-up questions remain outside the main task flow; answer each concisely with verified facts and no repetition. If all such questions fit naturally in the main sections, omit the FAQ section and document that decision and the questions covered in the QA report. Do not promise extra rankings from a FAQ heading or FAQ schema; Google no longer shows FAQ rich results in Search. Never invent search demand, pad the page with decorative questions, or duplicate answers merely to reach a question count.

Tables and checklists
Tables, checklists, and comparison grids are optional. Use them only when they help the reader compare, decide, verify, track, implement, or understand a process faster.

A “free template” promise must correspond to a real usable asset.

Practical-asset rule
When the topic benefits from one, create or propose a genuine asset such as:

downloadable checklist;
spreadsheet;
worksheet;
decision matrix;
incident-response form;
configuration audit sheet;
test procedure;
calculator;
security checker;
template.
The asset should reduce work for the reader, not simply duplicate article bullets in a PDF.

Cannibalization and cluster rules
Before proposing a new page:

check whether an existing page already owns the intent;
distinguish informational, comparison, setup, troubleshooting, and recovery intents;
prefer refreshing/expanding an existing page when the new topic would substantially overlap it;
keep clusters useful without endlessly expanding already-saturated subtopics.
For BizRiskGuide, do not over-expand MFA/email/password clusters merely because more keyword variants exist. Use actual gaps and GSC signals.

GSC feedback loop
After publishing, use Google Search Console data when available.

Review:

impressions;
clicks;
CTR;
average position;
queries;
page-level trends;
countries/devices when useful.
Use real query data to refine titles/meta, answer missing questions, strengthen internal links, update sections, and separate or consolidate intent when needed.

Do not interpret implementation completion as proof of ranking improvement.

Non-negotiable delivery gates
For a final article, verify article.md contains:

A separate publishing-settings block: exact focus keyword, separate WordPress Post Title/H1 and SEO plugin title, verified plugin suffix and final HTML title (or clearly marked unverified), meta description with counted characters, proposed slug and canonical URL, verified existing primary category and any justified secondary category, search intent, and secondary terms when useful.
A clean WordPress paste body with no # H1 or repeated post title when the theme renders the separate Post Title as H1; keyword in that title, introduction, relevant heading, body, and where natural conclusion or FAQ; readable prose and no editorial placeholders. For a standalone-document exception, include exactly one body H1 and explain its destination.
Contextual links to verified live internal pages and current authoritative external sources, with no UTM tracking parameters in proposed canonical/internal URLs; check target relevance, not only link syntax.
Practical implementation detail where useful: what to do, plan dependency, verification result, failure path, and evidence to save. Provide a usable worksheet/test record when it materially reduces reader work.
Verify the separate qa.md covers every gate in the required ledger, including source verification, real-world case outcome when relevant, links, taxonomy, FAQ decision, and limitations. Keep research notes and publishing instructions out of the article body.
If the user asks for only a revision of existing copy, preserve unrelated wording and structure, and explain any unavoidable change.

Ready-to-upload deliverable
When Abdul requests a final article:

clearly separate SEO settings from article body;
include SEO title;
meta description;
URL slug;
primary keyword;
suggested category when relevant;
clean article body;
contextual internal links;
authoritative external links;
sources/references when useful;
deliver as a real .md file by default for final articles; include a direct link to that file.
Do not place editorial notes inside the article body unless clearly marked for removal before publication.

Stop conditions
Never mark an article publish-ready if its Markdown file is missing, required on-page fields are absent, links are placeholders/unverified, a material current claim lacks a supporting source, the article duplicates an existing page’s intent without a defensible plan, or its supposed information gain is only a longer rewrite of competitors. Fix the issue if possible; otherwise disclose the precise blocker in the QA report. Do not turn a lack of paid keyword data into a fabricated difficulty score or ranking promise.

Final QA checklist
Before saying “ready to publish,” verify:

WordPress Post Title and article body are separate; the pasted body does not duplicate the rendered H1 (unless a verified template requires a body H1).
Every applicable workflow gate is reported with evidence from the final file; skipped gates have explicit N/A reasons.
Search intent is clear.
Page intent does not unnecessarily overlap an existing page.
Primary keyword appears naturally in key locations.
WordPress Post Title/H1 and SEO plugin title are separately optimized; final HTML title includes the verified plugin suffix once or is marked UNVERIFIED with a prepublication check.
Title is useful and click-worthy without misleading promises.
Meta description is within the agreed limit.
Facts and current-year details are verified.
Important claims have authoritative sources.
Internal links use final live URLs.
External links are useful and authoritative.
Article contains real information gain.
Semantic content review preserves one clear task, accurate relationships, and researched secondary questions answered without filler.
FAQ section is added only when it answers useful non-repetitive follow-ups; otherwise the QA explains which questions were covered in the main flow.
Practical steps are clear.
Verification/testing instructions are present where needed.
No fake experience, data, tests, or screenshots.
No filler added merely for word count.
Free-template/tool promises correspond to a real asset.
The article answers why a reader should prefer it after reading competing results.
Default BizRiskGuide editorial principles
Practical over theoretical.
Evidence over unsupported claims.
Clear over technical.
Specific over generic.
Useful differentiation over longer word count.
Small-business reality over enterprise-only advice.
Verification over “turn this on and hope.”
Original utility over copied SERP structure.
Trigger examples
Use this skill when Abdul says things such as:

“Use Maddy On Page SEO Skill.”
“Maddy SEO se topic research kro.”
“Is article ko Maddy SEO rules ke hisab se audit kro.”
“Competitors dekh kar information gain nikalo.”
“Ready-to-upload article bnao.”
“Is topic ko rankable angle do.”
“GSC data dekh kar article update kro.”
If Abdul explicitly overrides a rule for one task, follow that task-specific instruction while preserving the remaining skill rules.
