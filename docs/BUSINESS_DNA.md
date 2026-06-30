# Business DNA

Business DNA is the structured identity of a customer business.

It gives AI employees the context needed to produce useful, consistent, brand-safe work.

## Purpose

Business DNA should help the system understand:

- What the business sells.
- Who it serves.
- Why customers buy.
- How the brand speaks.
- What offers and services exist.
- What constraints and promises matter.
- Which languages, regions, and channels are relevant.

## Ownership

Client Template owns each customer's Business DNA.

Master Admin may define the schema, templates, defaults, package requirements, validation rules, and update strategy.

Business DNA should be editable by authorized customer users in the Client Template and visible to Master Admin only where support or administration requires it.

## Business Profile Model

The first Business DNA model should include these sections.

### Company Identity

- Business name.
- Legal or public brand name.
- Industry.
- Locations served.
- Website and primary contact points.
- Languages used with customers.

### Offers And Services

- Core offers.
- Services and products.
- Pricing notes, if relevant to marketing.
- Best-selling offers.
- Seasonal offers.
- Offer restrictions.
- Guarantee or promise.

### Target Audience

- Ideal customer profiles.
- Customer segments.
- Pain points.
- Buying triggers.
- Common objections.
- Customer sophistication level.
- Geographic or language constraints.

### Brand Voice

- Tone of voice.
- Words and phrases to use.
- Words and phrases to avoid.
- Formality level.
- Emotional style.
- Example approved copy.
- Example rejected copy.

### Competitors And Positioning

- Direct competitors.
- Indirect competitors.
- Differentiators.
- Market category.
- Proof points.
- Reasons customers choose this business.

### Calls To Action

- Primary CTA.
- Secondary CTAs.
- Booking links.
- Phone numbers.
- WhatsApp links.
- Lead forms.
- Landing page goals.

### Goals And Channels

- Marketing goals.
- Sales goals.
- Preferred channels.
- Existing channels.
- Content cadence.
- Campaign priorities.
- Success metrics.

### Assets

- Logos.
- Brand colors.
- Fonts.
- Product images.
- Service photos.
- Testimonials.
- Case studies.
- Videos.
- Existing landing pages.

### Restrictions

- Legal restrictions.
- Medical, financial, or regulated claims.
- Topics to avoid.
- Competitors not to mention.
- Promises not to make.
- Required disclaimers.
- Approval rules.

## Required Fields For First Build

The first build should require enough Business DNA to produce useful marketing drafts:

- Business name.
- Services or products.
- Target audience.
- Brand voice.
- Primary offer.
- Primary CTA.
- Languages.
- Restrictions.
- Marketing goals.

Optional fields can be added later without blocking onboarding.

## Versioning

Business DNA should be versioned because changes affect AI output quality and auditability.

Important changes should record:

- Version number.
- Changed fields.
- Editor.
- Timestamp.
- Reason for change.
- Whether prompt behavior may be affected.

## Validation

Business DNA should support validation rules, including:

- Required field completion.
- Supported language list.
- CTA format validation.
- Asset link validation.
- Restriction acknowledgement.
- Brand voice examples.

## AI Usage

Business DNA should feed prompt architecture, knowledge retrieval, employee behavior, content review, analytics interpretation, onboarding, and package eligibility.

Prompt packages should declare which Business DNA fields they require.

## Related Documents

- `PROMPT_ARCHITECTURE.md`
- `KNOWLEDGE_BASE.md`
- `AI_EMPLOYEES.md`
- `ONBOARDING.md`
- `ANALYTICS.md`
- `CLIENT_TEMPLATE.md`
- `MASTER_ADMIN.md`
