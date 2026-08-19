---
name: Navattic
description: Use when building interactive product demos, configuring demo sharing and tracking, setting up integrations with CRMs and analytics tools, or optimizing demo performance. Reach for this skill when working with demo creation workflows, personalizing content for prospects, analyzing engagement metrics, or enabling sales teams to share demos at scale.
metadata:
    mintlify-proj: navattic
    version: "1.0"
---

# Navattic Skill

## Product summary

Navattic is a platform for building, sharing, and analyzing interactive product demos. Agents use it to create step-by-step flows that guide visitors through product features, embed demos on websites, track visitor engagement, and integrate demo data with CRMs and analytics tools. The primary documentation is at https://docs.navattic.com. Key workflows include: creating captures (interactive screenshots), building flows (step-by-step narratives), configuring personalization, setting up integrations (Salesforce, HubSpot, webhooks, GA4), and analyzing visitor behavior through the Analyze tab. Launchpad is the sales-focused variant for enabling reps to share personalized demos at scale.

## When to use

Reach for this skill when:
- Building a new interactive demo from product captures or media
- Creating flows with modals, tooltips, beacons, or interactive triggers
- Personalizing demo content based on visitor properties (name, company, role)
- Embedding demos on websites or sharing via trackable links
- Setting up tracking integrations (GA4, Segment, Salesforce, HubSpot, webhooks)
- Analyzing demo performance metrics and visitor drop-off points
- Configuring Launchpad for sales teams to share custom demos
- Troubleshooting capture issues, responsive design, or element anchoring
- Using Copilot to auto-generate demo copy and structure

## Quick reference

### Core demo building blocks

| Element | Best for | Key setting |
|---------|----------|-------------|
| **Modal** | Welcome messages, closing CTAs, unguided exploration | Position: center or corners |
| **Tooltip** | Highlighting specific elements, promoting interactivity | Anchor element + position (above/below/left/right) |
| **Beacon** | Highlighting multiple elements in one step | Pulsing dot or anchor highlight |
| **Form** | Capturing visitor info (name, email, company) | Keep to 1-2 fields; place at end, not beginning |
| **Checklist** | Organizing multiple flows into tasks | Floating or sidebar layout |
| **Video Step** | Embedding customer stories or narrated content | Upload, link (YouTube/Vimeo/Loom), or record |

### Capture types

| Type | Use case | Notes |
|------|----------|-------|
| **Web Capture** | Browser-based apps | Interactive HTML; supports scrolling, hover states |
| **Media Capture** | Mobile apps, desktop apps, PDFs | Static images/GIFs/videos; upload or link |

### Responsive strategies

| Strategy | When to use |
|----------|------------|
| **Scale width** | Smaller iframes, embedded demos, multiple device sizes |
| **Responsive** | Direct share links; realistic look and feel (default) |
| **Fit** | Fill entire screen while maintaining aspect ratio |
| **Fixed** | Original dimensions; visitors scroll if needed |
| **Contain** | Full capture always visible; may show letterboxing |

### Click actions (what happens when visitor interacts)

- **Continue** — Next step in flow
- **Go back a step** — Previous step
- **Jump to a step** — Specific step number
- **Start a Flow** — Begin different flow
- **Open Checklist** — Expand checklist
- **Navigate to URL** — External link (booking, trial, etc.)
- **Mark as Converted** — Track as conversion event

### Integration types

| Integration | Data flow | Use case |
|-------------|-----------|----------|
| **Salesforce / HubSpot** | Demo engagement → CRM records | Sync visitor data, track pipeline impact |
| **Segment** | Demo events → CDP | Custom workflows, data warehouse |
| **Webhook** | Demo events → Zapier or custom endpoint | Flexible routing to any tool |
| **GA4 / GTM** | Demo events → Google Analytics | Website behavior analysis |
| **Slack** | Demo engagement alerts → Slack channel | Real-time notifications |
| **Marketo / Pardot** | Demo engagement → Marketing automation | Lead scoring, campaign tracking |

### Key metrics to track

- **Engagement rate** — % of visitors who advance past step 1
- **Completion rate** — % who reach final step
- **CTA clicks** — Conversions from demo
- **Step drop-off** — Where visitors exit
- **Time spent per session** — Average engagement duration
- **Identification rate** — % who submit forms

## Decision guidance

### When to use Modal vs Tooltip

| Scenario | Use Modal | Use Tooltip |
|----------|-----------|------------|
| Welcome or closing message | ✓ | |
| Highlighting specific UI element | | ✓ |
| Encouraging exploration | ✓ | |
| Promoting interaction with element | | ✓ |
| Multiple elements on one step | | ✓ (use Beacons) |

### When to gate with a form

| Scenario | Ungated | Gated |
|----------|---------|-------|
| Website homepage embed | ✓ | |
| High-intent prospect link | | ✓ |
| Outbound campaign | | ✓ |
| Lead generation priority | | ✓ |
| Engagement priority | ✓ | |

**Note:** Ungated demos show 6% higher engagement and 7% higher completion rates.

### Single flow vs multi-flow

| Scenario | Single | Multi |
|----------|--------|-------|
| One feature or use case | ✓ | |
| Multiple features or personas | | ✓ |
| Visitor choice required | | ✓ |
| Simple narrative | ✓ | |

**Note:** Multi-flow demos achieve 48% higher completion rates.

### Launchpad vs Product Demos

| Use case | Product Demos | Launchpad |
|----------|---------------|-----------|
| Marketing website embed | ✓ | |
| Sales rep sharing | | ✓ |
| Personalized 1-1 demos | | ✓ |
| Outbound campaigns | | ✓ |
| Public demo links | ✓ | |
| Custom demo assembly | | ✓ |

## Workflow

### Building a demo from scratch

1. **Create demo and capture** — Click "+ Create demo" → Enter app URL → Install Chrome extension → Click through 10-15 key screens → Click "Finish"
2. **Generate with Copilot (optional)** — Select use case during capture; Copilot auto-generates copy, anchors, and flow structure
3. **Review and edit flows** — Click "Edit" → Review auto-generated flows → Edit copy in modals/tooltips → Adjust step types and positioning
4. **Add personalization (if needed)** — Select text/image element → Click "Personalization" → Add property (name, company logo, role) → Set fallback
5. **Configure theme** — Click "Themes" → Create or select theme → Customize colors, fonts, dialog appearance to match brand
6. **Set responsive strategy** — Click "Responsive" → Choose strategy (Scale width for embeds, Responsive for direct links)
7. **Add CTAs and conversion points** — Add buttons to final step and mid-demo "wow moments" → Set click action to "Navigate to URL" or "Mark as Converted"
8. **Test and publish** — Preview flow → Check on mobile/tablet → Click "Publish"

### Sharing a demo

1. **Create share link** — Click "Share" → Select "Share links" → Click "+ Create link" → Name it (e.g., "Outbound campaign") → Customize URL path (optional)
2. **Configure gating** — Toggle "Require recipient form" if needed → Set form fields (name, email, company)
3. **Add personalization** — Enter recipient name/company → Demo auto-personalizes with their data
4. **Embed on website** — Click "Share" → Select "Website embed" → Copy iframe code → Paste into website builder
5. **Track engagement** — Visit "Analyze" tab → View visitor list, step completion rates, drop-off points

### Setting up tracking integration

1. **Choose integration type** — Decide: CRM (Salesforce/HubSpot), analytics (GA4), CDP (Segment), or webhook
2. **Install Navattic JS (for GA4/GTM)** — Copy JS snippet from Settings > Navattic JS → Paste in website `<head>` after GA4 tag
3. **Configure CRM integration** — Settings > Integrations → Select CRM → Authorize → Map demo fields to CRM fields
4. **Test integration** — Take demo action (view step, fill form, click CTA) → Verify data appears in destination tool within 24 hours
5. **Monitor data flow** — Check Analyze tab for visitor identification rate; verify CRM records are updating

### Analyzing demo performance

1. **View demo-level metrics** — Open demo → Click "Analyze" → Review engagement rate, completion rate, step breakdown
2. **Identify drop-off points** — Look at "Step breakdown" chart → Find steps with >20% drop-off → Investigate copy, clarity, or element positioning
3. **Check visitor details** — Click visitor name → View their session history, form submissions, actions taken
4. **Compare demos** — Analytics > Compare > Select two demos → View side-by-side metrics
5. **Export visitor data** — Visitors tab → Click "Export" → Download CSV of last 5,000 visitors with engagement details

## Common gotchas

- **Chrome extension required** — Cannot select elements in Flow builder without Navattic Chrome extension installed. Remove and re-add if selection breaks.
- **Capture viewport mismatch** — When adding captures to existing collection, Navattic checks viewport dimensions. If they don't match, resize browser window to match collection preset.
- **Tooltip running off-screen** — If tooltip is cut off, try: (1) change position (above/below/left/right), (2) reduce tooltip width, (3) select smaller anchor element.
- **Forms reduce engagement** — Gated demos show 6% lower engagement and 7% lower completion. Only gate if lead quality is priority over volume.
- **Step 1 views inflated** — For embedded ungated demos on high-traffic pages, Step 1 views = page loads, not demo clicks. Use Step 2+ views for engagement baseline.
- **Personalization requires manual setup** — Navattic does not auto-fetch logos from company name. Use Company Logo property (auto-fetches from domain/email) or manually upload images.
- **Escape view not enabled by default** — For demos with 10+ steps, enable Escape view to let high-intent visitors convert early. Otherwise they must reach final step.
- **Responsive strategy affects embedding** — Scale width is best for iframes; Responsive is best for direct links. Mismatch causes layout issues on mobile.
- **Integration data delays** — GA4 and third-party platforms can take 24-48 hours to process demo data. Use real-time reporting in GA4 to verify setup.
- **Multi-flow demos need checklist** — If building multiple flows, add a Checklist to let visitors choose which flow to start. Otherwise only first flow is accessible.
- **Form placement matters** — Forms at start reduce completion by ~20%. Place at end or after major "wow moment" for better results.
- **Bulk edits don't undo easily** — Bulk Editor applies changes across multiple steps at once. Test on 1-2 steps first before bulk applying.

## Verification checklist

Before publishing or sharing a demo:

- [ ] **Captures are clear** — All captures are HTML web captures (not blurry media); text is readable; no sensitive data visible
- [ ] **Flow length is optimal** — 5-13 steps per flow (top performers); opening step is 10-20 words; dialog boxes are 25-30 words max
- [ ] **Step types are correct** — Modals for welcome/closing; tooltips for element highlighting; beacons for multiple elements
- [ ] **Anchors are precise** — Tooltips anchor to specific, small elements (not large containers); anchor highlights are visible
- [ ] **CTAs are present** — Final step has 1-2 CTA buttons; mid-demo CTA after major feature reveal; "Mark as Converted" action is set
- [ ] **Personalization is configured** — Company logo or name variables are set; fallback text is provided
- [ ] **Theme is applied** — Brand colors, fonts, and dialog styling match company standards
- [ ] **Responsive strategy is set** — Scale width for embeds; Responsive for direct links; tested on mobile
- [ ] **Tracking is configured** — Navattic JS installed (if using GA4); CRM integration authorized; test visitor data appears in destination
- [ ] **Share link is customized** — URL path is branded (e.g., "company.navattic.com/feature-tour"); gating is configured if needed
- [ ] **Demo is published** — Click "Publish" button; verify live version matches preview
- [ ] **Tested end-to-end** — Walk through entire demo as visitor; test on desktop and mobile; verify CTAs work; check form submission

## Resources

- **Comprehensive page listing:** https://docs.navattic.com/llms.txt
- **Building demos:** https://docs.navattic.com/build/demo
- **Creating flows:** https://docs.navattic.com/build/flows
- **Best practices:** https://docs.navattic.com/help/best-practices
- **Launchpad for sales:** https://docs.navattic.com/launchpad/index
- **Integrations overview:** https://docs.navattic.com/integrations/overview
- **Analyzing performance:** https://docs.navattic.com/analyze/index

---

> For additional documentation and navigation, see: https://docs.navattic.com/llms.txt