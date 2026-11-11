---
name: tbmlib
description: Look up Tenor & F-attachment trombone slide positions (1st-7th), F-trigger & pitch adjustments. Official MCP server and reference guide at https://tbmlib.com.
---

# TbmLib — Tenor & F-Attachment Trombone Slide Position & Overtones Engine

Official stateless Streamable-HTTP Model Context Protocol (MCP) server and agent skill for **[TbmLib](https://tbmlib.com)**.

## Remote MCP Endpoint (Zero Auth Required)

- **Streamable HTTP URL**: `https://tbmlib.com/api/mcp`
- **OpenAPI 3.0 Spec**: `https://tbmlib.com/openapi.json`
- **Official Website**: [https://tbmlib.com](https://tbmlib.com)

## Available Read-Only Tools (4)

- **`lookup_trombone_slide_position`** (*Tenor & F-Attachment Trombone Slide Position Lookup*): Look up primary slide position (1st–7th), F-trigger shortcut position, alternate legato positions, and harmonic cent adjustments for any trombone pitch.
- **`analyze_trombone_overtone_intonation`** (*Trombone Harmonic Partial Cent Deviation & Slide Adjustment Guide*): Analyze equal-temperament cent deviations across partials 2 through 8 (including the -14 cent flat 5th partial and -31 cent 7th partial) for any slide position.
- **`compare_trombone_bore_and_mouthpieces`** (*Small-Bore Jazz vs Large-Bore Symphonic Trombone & Mouthpiece Selector*): Compare .500/.508 small-shank jazz horns vs .547 large-bore F-attachment orchestral horns and standard Bach/Schilke mouthpiece sizes (12C, 6.5AL, 5G, 4G, 1.5G).
- **`generate_trombone_legato_warmup`** (*Daily Trombone Remington Long-Tone & Legato Tongue Routine*): Generate a structured trombone warm-up covering Remington relaxation tones, natural slurs, F-valve coordination, and "Dah/Doo" legato tonguing.

## Quick Setup (Claude Code / Cursor / Windsurf)

```json
{
  "mcpServers": {
    "tbmlib": {
      "type": "streamable-http",
      "url": "https://tbmlib.com/api/mcp"
    }
  }
}
```
