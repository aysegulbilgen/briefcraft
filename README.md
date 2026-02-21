# BriefCraft

An AI agent skill that turns messy, unstructured inputs into clear, execution-ready briefs. Works with Claude Code, Cursor, GitHub Copilot, Cline, and any tool that supports the Agent Skills standard.

Teams often pass along half-finished notes, scattered Slack threads, or vague requests when they need a brief. BriefCraft takes that mess and transforms it into a structured document your team can actually act on.

## What it does

BriefCraft detects the right briefing mode, asks targeted questions to fill gaps, and outputs two things:

- A **Notion-style briefing page** with full detail
- A **Slack-ready summary** (8-12 lines) you can paste and share

## Modes

| Mode | From | To | Use when... |
|------|------|----|-------------|
| Product > Marketing | Product team | Marketing team | You have a feature or launch that Marketing needs to know about |
| Partnerships > Marketing | Partnerships team | Marketing team | You need to announce or co-market a partnership |
| Marketing > Agency | Marketing team | External agency | You are briefing an agency for creative or performance work |
| Marketing > Design | Marketing team | Design team | You need design assets and want to reduce revision loops |

## Install

```bash
npx skills add aysegulbilgen/briefcraft
```

## Usage

After installing, use the `/briefcraft` slash command in your AI coding tool:

```
/briefcraft
```

Paste your raw input (notes, Slack messages, docs, whatever you have). BriefCraft will:

1. Detect the right mode (or ask you)
2. Extract what is already known
3. Ask up to 10 targeted questions for anything missing
4. Generate both outputs

### Force a specific mode

Add a mode tag anywhere in your input:

- `[MODE: product]` for Product > Marketing
- `[MODE: partnership]` for Partnerships > Marketing
- `[MODE: agency]` for Marketing > Agency
- `[MODE: design]` for Marketing > Design

## Author

Built by [Aysegul](https://github.com/aysegulbilgen).

## License

MIT
