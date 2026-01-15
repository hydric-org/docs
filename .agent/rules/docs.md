---
trigger: always_on
---

This repository contains the source code for the hydric documentation, hosted at docs.hydric.org. hydric is a high-performance DeFi data layer that normalizes heterogeneous on-chain state into a unified financial model.

# Docs Provider & Infrastructure

This documentation is powered by [Mintlify](https://www.mintlify.com/).

- **Validation:** All suggestions must strictly adhere to the [Mintlify MDX components](https://mintlify.com/docs/components).
- **Automation:** The API reference is synchronized with our OpenAPI (Swagger) specification. Do not manually hardcode data that is available in the `openapi.json` located remotely at (https://api.hydric.org/v1/openapi.json)
- **Naming:** Always use **hydric** lowercased, as it's part of the branding. Use "Indexing Layer" and "Gateway Layer" consistently.

# The "Elite" Standard (Design Principles)

The goal is to achieve high-level engineering clarity. Follow these principles for every page:

1. **Truthful Authority:** Be precise. Do not use marketing fluff. Explain the "Why" through engineering reality (e.g., "Semantic Normalization" instead of "Clean Data").
2. **Scannability:** Use bolding, bullet points, and horizontal rules (`---`) to break up dense text. A developer should understand the value of a page in 5 seconds.
3. **Outcome-Oriented:** Every technical page should focus on the **utility** for the integrator.
4. **Developer Empathy:** Acknowledge the complexity of DeFi and explain how hydric specifically collapses that complexity.

# Content Hierarchy & Voice

- **The Vision:** Frame hydric as a "Primitive-Centric" system. We treat DeFi as fundamental financial behaviors (Liquidity Pools, Lending Markets, Activity).
- **Voice:** Professional, insightful, and helpful. Use a "Technical Peer" tone, not a rigid lecturer or a salesperson.
- **Visuals:** Whenever a complex system is described, suggest a diagram or a Mermaid flow to illustrate the data lifecycle.

# Mintlify-Specific Requirements

- **Metadata:** Every `.mdx` file must start with a `title` and `description` in the frontmatter.
- **Components:** Use `<ResponseField>`, `<Expandable>`, and `<Note>` to highlight key information.
- **Snippets:** For content used across multiple pages (like the Pool Schema Example), use Mintlify Snippets to maintain a single source of truth.
- **API Integration:** Use the `openapi` attribute in frontmatter to link MDX pages directly to our Swagger DTOs.

# Quality Checklist

Before finalizing any change, verify:

- Is the language "Elite" and grammatically perfect?
- Is the information technically accurate regarding the Indexing and Gateway layers?
- Does it link back to the "Standard Schema" where relevant?
- Is there a clear "Next Step" or "Call to Action" for the user?
