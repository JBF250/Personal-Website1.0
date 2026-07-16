---
name: awesome-design-md
description: "Curated collection of DESIGN.md files for 73+ brands. Each file contains complete design system specifications including colors, typography, components, layout principles, and responsive behavior. Use these DESIGN.md files to generate high-quality, consistent UI that matches the visual language of real-world websites."
license: MIT
---

# Awesome DESIGN.md

## Overview

DESIGN.md is a plain-text design system document format introduced by Google Stitch. AI agents read these files to understand how UI should look and feel. This skill provides 73+ ready-to-use DESIGN.md files extracted from real websites, enabling consistent UI generation across different brand design languages.

## Quick Reference

| Task | Approach |
|------|----------|
| List available brands | Run `powershell -ExecutionPolicy Bypass -File scripts/list-brands.ps1` or check the `design-md/` directory |
| Copy a DESIGN.md to project | Use `powershell -ExecutionPolicy Bypass -File scripts/copy-design.ps1 -brand apple` |
| Search brands by category | Use `powershell -ExecutionPolicy Bypass -File scripts/search-brands.ps1 -category "AI & LLM Platforms"` |

## Available Brands

### AI & LLM Platforms
- claude, cohere, elevenlabs, minimax, mistral.ai, ollama, opencode.ai, replicate, runwayml, together.ai, voltagent, x.ai

### Developer Tools & IDEs
- cursor, expo, lovable, raycast, superhuman, vercel, warp

### Backend, Database & DevOps
- clickhouse, composio, hashicorp, mongodb, posthog, sanity, sentry, supabase

### Productivity & SaaS
- cal, intercom, linear.app, mintlify, notion, resend, zapier

### Design & Creative Tools
- airtable, clay, figma, framer, miro, webflow

### Fintech & Crypto
- binance, coinbase, kraken, mastercard, revolut, stripe, wise

### E-commerce & Retail
- airbnb, meta, nike, shopify, starbucks

### Media & Consumer Tech
- apple, hp, ibm, nvidia, pinterest, playstation, spacex, spotify, theverge, uber, vodafone, wired

### Automotive
- bmw, bmw-m, bugatti, ferrari, lamborghini, renault, tesla

### Retro Web
- dell-1996, nintendo-2001

## What's Inside Each DESIGN.md

Every file follows the [Stitch DESIGN.md format](https://stitch.withgoogle.com/docs/design-md/specification/) with extended sections:

| Section | What it captures |
|---------|-----------------|
| Visual Theme & Atmosphere | Mood, density, design philosophy |
| Color Palette & Roles | Semantic name + hex + functional role |
| Typography Rules | Font families, full hierarchy table |
| Component Stylings | Buttons, cards, inputs, navigation with states |
| Layout Principles | Spacing scale, grid, whitespace philosophy |
| Depth & Elevation | Shadow system, surface hierarchy |
| Do's and Don'ts | Design guardrails and anti-patterns |
| Responsive Behavior | Breakpoints, touch targets, collapsing strategy |
| Agent Prompt Guide | Quick color reference, ready-to-use prompts |

## Usage

### Method 1: Direct Copy
Copy the desired DESIGN.md from `design-md/<brand>/DESIGN.md` to your project root.

### Method 2: PowerShell Script
```powershell
# List all available brands
powershell -ExecutionPolicy Bypass -File scripts/list-brands.ps1

# Copy Apple DESIGN.md to current directory
powershell -ExecutionPolicy Bypass -File scripts/copy-design.ps1 -brand apple

# Copy multiple brands
powershell -ExecutionPolicy Bypass -File scripts/copy-design.ps1 -brand apple, stripe, vercel

# Search brands by keyword
powershell -ExecutionPolicy Bypass -File scripts/search-brands.ps1 -keyword "dark"
```

**Note**: If PowerShell execution policy blocks the scripts, use `-ExecutionPolicy Bypass` as shown above.

### Method 3: Use in Projects
1. Copy a site's `DESIGN.md` into your project root
2. Tell your AI agent to use it when generating UI
3. Example prompt: "Build me a landing page that looks like Apple's website"

## File Structure

```
awesome-design-md/
├── SKILL.md
├── LICENSE
├── design-md/
│   ├── apple/
│   │   ├── DESIGN.md
│   │   └── README.md
│   ├── stripe/
│   │   ├── DESIGN.md
│   │   └── README.md
│   └── ... (73+ brands)
└── scripts/
    ├── list-brands.ps1
    ├── copy-design.ps1
    └── search-brands.ps1
```

## Dependencies

No external dependencies required. All DESIGN.md files are plain text and can be read directly by AI agents.

## License

MIT License - see LICENSE for details.

This repository is a curated collection of design system documents extracted from public websites. All DESIGN.md files are provided "as is" without warranty. The extracted design tokens represent publicly visible CSS values.