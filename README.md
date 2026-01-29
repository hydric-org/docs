# hydric Documentation

### The Knowledge Layer for the Unified Financial Model

This repository houses the source of truth for **docs.hydric.org**. It contains the technical specifications, integration guides, and API references for the Hydric Gateway.

Powered by **Mintlify**.

---

## The Documentation Thesis

Just like our API, our documentation follows strict engineering principles. It is not marketing material; it is a **Technical Contract**.

1. **Precision over Fluff:** We do not use "marketing speak." We define fields by their data type, precision (e.g., Q64.96), and source.
2. **Component-Driven:** We use shared snippets (e.g., `supported-blockchains.mdx`, `error-table.mdx`) to ensure that the docs never drift from the codebase.
3. **Primitive-Based Organization:** Content is organized by Financial Primitive (Liquidity Pools, Lending, Staking), not by individual protocol, reflecting the Hydric normalization strategy.

## Local Development

### Prerequisites

- **Mintlify CLI**

### Installation

```bash
npm i -g mintlify
```

### Running Locally

To preview the documentation with hot-reloading:

```bash
mintlify dev
```

The documentation will be available at http://localhost:3000.

## Repository Structure

/api-reference
The OpenAPI (Swagger) definitions and endpoint documentation.
NOTE: Much of this is synced automatically from the Gateway DTOs.

/snippets
Reusable MDX components (Error codes, Network lists) used to keep the docs DRY.

docs.json
The configuration file for navigation structure, visual theming, and redirects.
