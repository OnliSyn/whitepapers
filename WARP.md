# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Repository Overview

This is a documentation repository containing technical whitepapers for the ONLI Architecture—a digital asset management system based on law-preserving computation and the Physics of Finance principles. The repository focuses on academic and business documentation rather than code.

**Core Content:**
- Whitepaper series explaining ONLI's architecture and use cases
- Market analysis and cost comparisons
- Technical documentation on Genomes, Genes, Vaults, and tensor-based uniqueness

**Note:** The `old.gitignore/` directory contains deprecated versions and should be ignored when working with current documentation. The `brandimages/` folder contains visual assets and should also be ignored.

## Document Structure

The whitepapers follow a versioned naming convention:

1. **01_Revolution-v40.md** - Core architecture paper introducing ONLI's paradigm shift from access control to law-preserving computation
2. **02_Usecase-Guide-v21.md** - Practical implementation guide for enterprises deploying ONLI
3. **03_Market-Oppty-v31.md** - Market opportunity analysis ($17T TAM across stablecoins, RWAs, crypto infrastructure, OTC derivatives)
4. **05_Uniqueness-Quant-v31.md** - Technical deep-dive on the Uniqueness-Quantification Problem and tensor-based solutions
5. **Cost-Comparison-v31.md** - Economic analysis showing 62-81% cost savings vs blockchain
6. **Sutton-Selects-v21.md** - Real-world use case demonstrating actual possession technology in supply chain finance

## Key Terminology and Concepts

When working with these documents, understand these core ONLI concepts:

- **Genomes**: Tensor-based digital assets with cryptographic identity (not files or ledger entries)
- **Genes**: Hardware-protected ownership credentials bound to legal identities (not private keys)
- **Vaults**: Trusted execution environments (TEEs) enforcing hardware-level possession
- **Physics of Finance**: Four principles requiring legal identity, enforceability, issuer liability, and accounting assertions
- **Uniqueness-Quantification Problem**: The challenge of proving digital objects are architecturally singular
- **Law-Preserving Computation**: Architecture designed to satisfy property law, accounting standards, and regulatory requirements
- **Ledger Fallacy**: The blockchain misconception that records about ownership create ownership itself
- **Actual Possession Model**: ONLI's approach where assets exist as singular objects vs blockchain's distributed consensus model

## Document Consistency Guidelines

When editing or creating new content:

1. **Version Alignment**: All documents reference "ONLI Architecture Framework" and should maintain consistency with the v3.x/v4.x architecture
2. **Terminology**: Use ONLI-specific terms consistently (Genome/Gene/Vault, not token/key/wallet)
3. **Core Narrative**: Maintain the central thesis that digital property requires architectural alignment with legal principles, not just engineering optimization
4. **Comparative Analysis**: When comparing to alternatives, focus on blockchain (distributed consensus) vs ONLI (actual possession) and traditional systems (custodial access)
5. **Financial Framing**: Emphasize regulatory compliance (IFRS 9, US GAAP), accounting assertions, and the Physics of Finance
6. **Avoid Generic Claims**: Don't add generic development advice—these are specialized technical/business documents

## Marketplace Platform Context

The project includes a specific marketplace implementation with these account roles:
- **Treasury**: Assurance Account (USDT for stability) and Inventory Account (Specie for reserve)
- **Marketplace Operator**: Funding Account (USDT) for fee collection
- **LiquidityProvider**: Funding Account (USDT) for redemption fees
- **Users**: Funding Account (USDT) for transactions, plus Incoming/Outgoing Bank Accounts (USD ACH)

Fee structure:
- No transaction fees
- Issuance fees: 5% of $1 Specie principal to Marketplace Operator
- Listing fees: $100 USDT for listings ≥ 5,000 Specie
- Redemption fee: 1% to LiquidityProvider

Key statistics: Price ($1.00), Market Inventory (Specie listed for sale), Stability Ratio (Assurance balance over circulation)

## Working with This Repository

**Reading Documents:**
- Start with 01_Revolution for architectural overview
- Use 02_Usecase-Guide for practical implementation context
- Reference 05_Uniqueness-Quant for technical depth

**Creating New Content:**
- Follow the versioned naming pattern: `##_Title-v##.md`
- Include standard header: Author, Version, Date, Abstract, Executive Summary
- Maintain academic/professional tone with technical precision
- Cross-reference other whitepapers in References section

**Updating Existing Documents:**
- Increment version number in filename and header
- Add "Updated: [Date] (Version X.X)" line in header
- Maintain consistency with Physics of Finance principles
- Preserve existing structure (Abstract → Executive Summary → Numbered Sections → References)

## Important Notes

- This is a documentation repository—there is no build, test, or deployment process
- Changes are typically reviewed for technical accuracy and terminology consistency
- All whitepapers assume reader familiarity with blockchain, databases, and property law fundamentals
