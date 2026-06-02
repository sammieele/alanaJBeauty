# Alana J-Beauty Tab - Verified Shelf Strategy and UI Prototype

This repository presents the recommended direction for Alana's J-Beauty launch:

1. Trust-first discovery in Discover
2. Product-level verification transparency
3. A persistent personal shelf designed for repeat purchasing

The concept is a hybrid of Concept 1 and Concept 3, with Ask Alana Expert (Concept 2) positioned as a progressive enhancement in Phase 2.

## Executive Recommendation

The strongest direction is Verified Shelf: a J-Beauty section inside Discover, anchored by the Alana Verified badge system and connected to a persistent personal shelf.

Why this is the right move:
- It starts from Alana's unique advantage: trusted sourcing plus AI assistance.
- It delivers immediate value to JETRO partners by making SME credibility visible at first glance.
- It creates a repeat-purchase loop from day one through saved products and reorder behavior.
- It keeps Phase 1 engineering scope tight by reusing existing Alana UI and infrastructure patterns.

## Strategic Fit with JETRO Goals

Verified Shelf maps directly to JETRO outcomes:
- Increase SME export visibility: weekly Drops spotlight new Japanese brands in a recurring format.
- Drive repeat international purchasing: Shelf persistence turns one-time discovery into ongoing reorder behavior.
- Build trusted commerce infrastructure: Alana Verified badge and disclosure create transparent sourcing signals at the point of intent.

## User Value Proposition

The experience solves two core user problems in one flow:
- Trust problem: users need confidence that products are authentic and sourced from authorized channels.
- Memory problem: users need a simple way to remember and repurchase products they liked.

Verified Badge solves trust at product-card level. Shelf solves memory across sessions. Together, they position Alana as a beauty relationship manager, not just a discovery feed.

## Product and Design Principles

This direction fits current Alana patterns without requiring a visual reset:
- Discover remains the primary entry surface.
- Existing card and tab primitives are reused.
- Green trust cues and clean surfaces remain consistent with brand language.
- J-Beauty identity is expressed through bilingual naming and editorial content, not a new design system.

## Engineering Scope and Feasibility

Phase 1 workstreams are bounded and parallelizable:
- Verified Badge: metadata attribute plus badge UI and disclosure sheet.
- J-Beauty Discover section: curated feed state inside current navigation structure.
- Shelf foundation: saved products, shelf screen, and reorder links.
- Weekly Drop: content operation using curated collections and existing feed rendering.

No new checkout stack is required for Phase 1.

## Roadmap

### Phase 1 (MVP): Make Trusted Commerce Real
- Launch J-Beauty section in Discover
- Ship Alana Verified badge + bottom-sheet disclosure
- Ship persistent My J-Beauty Shelf with save and reorder entry points
- Ship weekly editorial Drop module

### Phase 2: Add Intelligence and Scale
- Add Ask Alana Expert mode as guided entry point
- Add reorder intelligence and low-stock prompts
- Add K-Beauty catalog using the same shelf and badge architecture
- Add regional selector at section level (J-Beauty / K-Beauty)

### Phase 3: Unified Asian Beauty
- Promote regional selector as primary sub-navigation
- Evolve section into Asian Beauty using shared trust, shelf, and AI layers

## Screen-by-Screen Walkthrough

Target narrative for stakeholder review is five screens.

### 1. J-Beauty entry in Discover
- User lands in a focused section, not a broad catalog.
- Primary content: weekly Drop, shelf entry point, featured brands.
- Top filter can expand over time (All / J-Beauty / K-Beauty).

### 2. Product detail with Alana Verified badge
- Badge appears next to brand identity, not buried in details.
- Buy CTA reinforces trust context: buy from verified retailer.
- Product detail supports bilingual naming cues for authenticity.

### 3. Badge disclosure bottom sheet
- Tap badge to view plain-language sourcing and authorization details.
- Disclosure pattern turns trusted commerce framework into visible UX.

### 4. My J-Beauty Shelf
- Persistent saved collection across sessions.
- Fast reorder path per product.
- Foundation for repeat purchase behavior and retention.

### 5. Shelf intelligence states
- Contextual low-stock and reorder nudges.
- Add-from-drop pathways to connect discovery and repeat purchase.

## Prototype Coverage in This Repository

Current files cover the core Phase 1 interactions and shelf intelligence cue:
- `alana_screens_redesigned.html` - Combined showcase (recommended entry point)
- `screen1_jbeauty_entry.html` - Discover entry and Drop framing
- `screen2_product_card_and_badge.html` - Product detail + badge disclosure
- `screen3_my_shelf.html` - Persistent shelf with reorder and alert state

## Design System Notes

The prototype uses tokenized styles in `:root` to keep visuals consistent across screens:
- Brand greens for trust and verification cues
- Neutral layered surfaces for card hierarchy
- Reusable mobile frame, spacing, and card primitives
- Shared badge and disclosure components

## Quick Start

No build step is required.

1. Clone or download this folder.
2. Open `alana_screens_redesigned.html` in a browser.

Optional (VS Code Live Server):
- Right-click `alana_screens_redesigned.html`
- Select Open with Live Server

## Dependency

- Tabler Icons Webfont via CDN: https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@3.10.0/dist/tabler-icons.min.css

An internet connection is required to load CDN-hosted icons.

## Next Implementation Steps

- Add lightweight interaction logic (tab state, badge-sheet toggle, save state)
- Persist shelf items to user account storage
- Add CMS fields for Drop metadata and verification copy
- Add accessibility polish (focus states, ARIA labels, keyboard sheet dismissal)
- Add analytics events for trust interactions and reorder funnels

## License

This prototype is intended for internal strategy, design, and product review unless a separate license is provided.
# Alana J-Beauty Tab - Verified Shelf Strategy and UI Prototype

This repository presents the recommended direction for Alana's J-Beauty launch:

1. Trust-first discovery in Discover
2. Product-level verification transparency
3. A persistent personal shelf designed for repeat purchasing

The concept is a hybrid of Concept 1 and Concept 3, with Ask Alana Expert (Concept 2) positioned as a progressive enhancement in Phase 2.

## Executive Recommendation

The strongest direction is Verified Shelf: a J-Beauty section inside Discover, anchored by the Alana Verified badge system and connected to a persistent personal shelf.

Why this is the right move:
- It starts from Alana's unique advantage: trusted sourcing plus AI assistance.
- It delivers immediate value to JETRO partners by making SME credibility visible at first glance.
- It creates a repeat-purchase loop from day one through saved products and reorder behavior.
- It keeps Phase 1 engineering scope tight by reusing existing Alana UI and infrastructure patterns.

## Strategic Fit with JETRO Goals

Verified Shelf maps directly to JETRO outcomes:
- Increase SME export visibility: weekly Drops spotlight new Japanese brands in a recurring format.
- Drive repeat international purchasing: Shelf persistence turns one-time discovery into ongoing reorder behavior.
- Build trusted commerce infrastructure: Alana Verified badge and disclosure create transparent sourcing signals at the point of intent.

## User Value Proposition

The experience solves two core user problems in one flow:
- Trust problem: users need confidence that products are authentic and sourced from authorized channels.
- Memory problem: users need a simple way to remember and repurchase products they liked.

Verified Badge solves trust at product-card level. Shelf solves memory across sessions. Together, they position Alana as a beauty relationship manager, not just a discovery feed.

## Product and Design Principles

This direction fits current Alana patterns without requiring a visual reset:
- Discover remains the primary entry surface.
- Existing card and tab primitives are reused.
- Green trust cues and clean surfaces remain consistent with brand language.
- J-Beauty identity is expressed through bilingual naming and editorial content, not a new design system.

## Engineering Scope and Feasibility

Phase 1 workstreams are bounded and parallelizable:
- Verified Badge: metadata attribute plus badge UI and disclosure sheet.
- J-Beauty Discover section: curated feed state inside current navigation structure.
- Shelf foundation: saved products, shelf screen, and reorder links.
- Weekly Drop: content operation using curated collections and existing feed rendering.

No new checkout stack is required for Phase 1.

## Roadmap

### Phase 1 (MVP): Make Trusted Commerce Real
- Launch J-Beauty section in Discover
- Ship Alana Verified badge + bottom-sheet disclosure
- Ship persistent My J-Beauty Shelf with save and reorder entry points
- Ship weekly editorial Drop module

### Phase 2: Add Intelligence and Scale
- Add Ask Alana Expert mode as guided entry point
- Add reorder intelligence and low-stock prompts
- Add K-Beauty catalog using the same shelf and badge architecture
- Add regional selector at section level (J-Beauty / K-Beauty)

### Phase 3: Unified Asian Beauty
- Promote regional selector as primary sub-navigation
- Evolve section into Asian Beauty using shared trust, shelf, and AI layers

## Screen-by-Screen Walkthrough

Target narrative for stakeholder review is five screens.

### 1. J-Beauty entry in Discover
- User lands in a focused section, not a broad catalog.
- Primary content: weekly Drop, shelf entry point, featured brands.
- Top filter can expand over time (All / J-Beauty / K-Beauty).

### 2. Product detail with Alana Verified badge
- Badge appears next to brand identity, not buried in details.
- Buy CTA reinforces trust context: buy from verified retailer.
- Product detail supports bilingual naming cues for authenticity.

### 3. Badge disclosure bottom sheet
- Tap badge to view plain-language sourcing and authorization details.
- Disclosure pattern turns trusted commerce framework into visible UX.

### 4. My J-Beauty Shelf
- Persistent saved collection across sessions.
- Fast reorder path per product.
- Foundation for repeat purchase behavior and retention.

### 5. Shelf intelligence states
- Contextual low-stock and reorder nudges.
- Add-from-drop pathways to connect discovery and repeat purchase.

## Prototype Coverage in This Repository

Current files cover the core Phase 1 interactions and shelf intelligence cue:
- `alana_screens_redesigned.html` - Combined showcase (recommended entry point)
- `screen1_jbeauty_entry.html` - Discover entry and Drop framing
- `screen2_product_card_and_badge.html` - Product detail + badge disclosure
- `screen3_my_shelf.html` - Persistent shelf with reorder and alert state

## Design System Notes

The prototype uses tokenized styles in `:root` to keep visuals consistent across screens:
- Brand greens for trust and verification cues
- Neutral layered surfaces for card hierarchy
- Reusable mobile frame, spacing, and card primitives
- Shared badge and disclosure components

## Quick Start

No build step is required.

1. Clone or download this folder.
2. Open `alana_screens_redesigned.html` in a browser.

Optional (VS Code Live Server):
- Right-click `alana_screens_redesigned.html`
- Select Open with Live Server

## Dependency

- Tabler Icons Webfont via CDN: https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@3.10.0/dist/tabler-icons.min.css

An internet connection is required to load CDN-hosted icons.

## Next Implementation Steps

- Add lightweight interaction logic (tab state, badge-sheet toggle, save state)
- Persist shelf items to user account storage
- Add CMS fields for Drop metadata and verification copy
- Add accessibility polish (focus states, ARIA labels, keyboard sheet dismissal)
- Add analytics events for trust interactions and reorder funnels

## License

This prototype is intended for internal strategy, design, and product review unless a separate license is provided.
