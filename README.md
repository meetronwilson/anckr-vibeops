# Turf Assistant 2.0 - Product Contracts

This repository contains the product contracts (modules and features) for **Turf Assistant 2.0**, a code-first, AI-assistant-led turf management system.

## Overview

Turf Assistant 2.0 is designed with an "open-first brain" approach where an AI assistant guides users through daily operations, providing proactive recommendations and automating routine decisions.

**Key Principles:**
- **Hours, not Weeks:** Rapid onboarding and time-to-value
- **Code-First:** Focus on building, not planning documents
- **Open-First Brain:** AI assistant leads the experience
- **Minimalist:** Essential features only, removing APEX complexity
- **Syngenta-First:** Products catalog and sensor integration prioritized

## Structure

```
.vibeops/
├── modules/           # 11 module contracts
├── features/          # 54 feature contracts
├── issues/            # Feature issues and tasks
├── schemas/           # JSON schemas for validation
├── templates/         # Contract templates
└── README.md          # Documentation
```

## Modules (11)

1. **MOD-001:** Assistant Core (Open-First Brain) - 6 features
2. **MOD-002:** Applications (Agronomy) - 6 features
3. **MOD-003:** Labor & Scheduling (Minimalist) - 5 features
4. **MOD-004:** Mapping & Irrigation - 5 features
5. **MOD-005:** Expenses & Budget - 5 features
6. **MOD-006:** Integrations - 5 features
7. **MOD-007:** Onboarding (Hours, not Weeks) - 5 features
8. **MOD-008:** Communications & Staff Experience - 4 features
9. **MOD-009:** Analytics & Reporting - 4 features
10. **MOD-010:** Platform & Security (MakerKit Base) - 5 features
11. **MOD-011:** Admin & Partner Ops - 4 features

**Total Features:** 54

## Getting Started

This project uses the [VibeOps MCP Server](https://github.com/vibeops/product-os) for managing product contracts with Claude Code.

### Installation

```bash
# Install dependencies
npm install

# Add VibeOps MCP server to Claude Code
claude mcp add --transport stdio --scope local vibeops -- node node_modules/@anckr/vibeops/build/index.js

# Verify setup
claude mcp list
```

### Usage with Claude Code

Once the MCP server is configured, you can:
- Create and manage modules
- Define feature contracts with PRDs
- Track issues and user stories
- Generate implementation artifacts

## Key Features Highlights

### Assistant Core
- Morning Brief (≤5 minutes)
- Proactive Scheduling with 1-click accept
- Application Proposals from triggers
- Natural Language I/O (chat + SMS)
- Confirm-to-Execute guardrails

### Onboarding
- Create Course Wizard (≤2 hours setup)
- CSV Templates for bulk import
- KML Drop for rapid mapping
- First-Run Assistant
- Seeded Demo (≤30 seconds)

### Agronomy
- Syngenta-first Products Catalog
- GDD/Weather/Disease Triggers Engine
- Auto-generated Recipe Cards
- Compliance Ledger

## Deferred/Removed

- **APEX:** Removed (micromanagement tool)
- **Fleet:** Deferred (post-MVP consideration)

## Technology Stack

- **Foundation:** MakerKit (Next.js, Supabase)
- **AI:** Claude integration for assistant
- **SMS:** Twilio
- **Email:** SendGrid
- **Payments:** Stripe
- **Maps:** GIS libraries for KML/GeoJSON

## Contributing

Product contracts follow the VibeOps structure:
- Modules define high-level initiatives
- Features contain detailed PRDs
- Issues track implementation tasks

## License

MIT

---

**Built with ❤️ for golf course superintendents**
