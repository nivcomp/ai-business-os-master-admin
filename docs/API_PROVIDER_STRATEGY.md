# API Provider Strategy

AI Business OS should connect AI employees to the best available APIs through a provider layer, not through hard-coded vendor logic.

## Strategic Goal

The platform should let the company sell business employees while quietly connecting those employees to strong APIs for text, image, video, voice, publishing, analytics, CRM, messaging, and automation.

Customers buy outcomes and employees. Internally, each employee may use multiple provider adapters.

## Provider Principles

- Use provider adapters instead of direct vendor coupling.
- Choose providers by output quality, reliability, cost, speed, and replacement risk.
- Support swapping providers without rewriting product workflows.
- Keep provider keys secure and scoped by client or platform owner.
- Require approval before provider-driven actions publish, send, delete, charge, or expose data.

## Provider Categories

### Text And Reasoning

Used for copywriting, planning, campaign strategy, SEO briefs, content editing, analytics summaries, and support drafts.

Capabilities:

- Generate structured text.
- Rewrite or improve text.
- Summarize records.
- Extract structured fields.
- Classify approval or risk state.
- Produce JSON-compatible workflow output.

### Image Generation And Editing

Used by Designer employees for ad concepts, social images, product visuals, thumbnails, and brand assets.

Capabilities:

- Generate images from prompt.
- Edit existing images.
- Create brand-consistent variations.
- Resize or adapt aspect ratios.
- Produce metadata for approval and reuse.

### Video Generation And Editing

Used by Video Creator employees for short-form concepts, reels, ad variations, explainers, and campaign video drafts.

Capabilities:

- Generate video from prompt.
- Generate video from image.
- Produce captions or scripts.
- Create short clips for social channels.
- Export status and asset URLs.

### Voice And Audio

Used for voiceover, ad narration, podcast snippets, phone scripts, and future support or sales employees.

Capabilities:

- Text to speech.
- Speech to text.
- Voice style selection.
- Language support.
- Consent and rights metadata.

### Publishing And Scheduling

Used by Campaign Manager employees to prepare or publish content to external channels.

Capabilities:

- Prepare social post drafts.
- Schedule approved content.
- Publish approved content.
- Retrieve publish status.
- Capture errors and channel constraints.

Publishing actions should require human approval by default.

### CRM And Leads

Used by CRM Lite, Sales employees, Marketing Manager, and Campaign Manager.

Capabilities:

- Create or update leads.
- Read contact context.
- Track campaign source.
- Record follow-up tasks.
- Sync simple pipeline state.

### Messaging

Used for WhatsApp, email, SMS, and future customer communication workflows.

Capabilities:

- Prepare message drafts.
- Send approved messages.
- Track delivery state.
- Respect unsubscribe and consent rules.
- Record message history.

### Analytics

Used by Analytics Manager and Master Admin client health.

Capabilities:

- Fetch campaign metrics.
- Fetch website or landing page metrics.
- Track product usage events.
- Summarize performance.
- Recommend improvements.

## Provider Registry

Master Admin should maintain a provider registry with:

- Provider name.
- Category.
- Capabilities.
- Credential requirements.
- Cost model.
- Rate limits.
- Supported environments.
- Replacement candidates.
- Security notes.
- Approval requirements.

## First Build Recommendation

For the MVP, do not connect every provider immediately.

Start with provider interfaces and mock or placeholder adapters for:

- Text generation.
- Image generation.
- Video generation.
- Social publishing.
- Analytics.
- CRM Lite.

Then connect real providers one category at a time as workflows become sellable.

## Related Documents

- `PROVIDER_LAYER.md`
- `TOOLS.md`
- `AI_EMPLOYEES.md`
- `MARKETING_AUTOMATION_ENGINE.md`
- `SECURITY.md`
- `MVP_BUILD_PLAN.md`
