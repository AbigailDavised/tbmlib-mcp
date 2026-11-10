# TbmLib — Tenor & F-Attachment Trombone Slide Position & Overtones Engine

[![Official Website](https://img.shields.io/badge/Website-tbmlib.com-blue)](https://tbmlib.com)
[![MCP Registry](https://img.shields.io/badge/MCP_Registry-com.tbmlib%2Fmcp-green)](https://www.mcptry.com/servers/com.tbmlib/mcp)
[![Glama Connector](https://img.shields.io/badge/Glama-Connector-purple)](https://glama.ai/mcp/connectors/com.tbmlib/mcp)

Look up Tenor & F-attachment trombone slide positions (1st-7th), F-trigger & pitch adjustments.

- **Official Workbench**: [https://tbmlib.com](https://tbmlib.com)
- **Remote MCP Endpoint**: `https://tbmlib.com/api/mcp` (`streamable-http`, read-only, no API key required)
- **Public OpenAPI 3.0**: [https://tbmlib.com/openapi.json](https://tbmlib.com/openapi.json)
- **LLM Context**: [https://tbmlib.com/llms.txt](https://tbmlib.com/llms.txt) · [https://tbmlib.com/llms-full.txt](https://tbmlib.com/llms-full.txt)

## Tools Provided (4 Read-Only Tools)

| Tool Name | Summary |
| :--- | :--- |
| `lookup_trombone_slide_position` | Look up primary slide position (1st–7th), F-trigger shortcut position, alternate legato positions, and harmonic cent adjustments for any trombone pitch. |
| `analyze_trombone_overtone_intonation` | Analyze equal-temperament cent deviations across partials 2 through 8 (including the -14 cent flat 5th partial and -31 cent 7th partial) for any slide position. |
| `compare_trombone_bore_and_mouthpieces` | Compare .500/.508 small-shank jazz horns vs .547 large-bore F-attachment orchestral horns and standard Bach/Schilke mouthpiece sizes (12C, 6.5AL, 5G, 4G, 1.5G). |
| `generate_trombone_legato_warmup` | Generate a structured trombone warm-up covering Remington relaxation tones, natural slurs, F-valve coordination, and "Dah/Doo" legato tonguing. |

## Connect in 10 Seconds

### Claude Code
```bash
claude mcp add --transport http tbmlib https://tbmlib.com/api/mcp
```

### Cursor / Claude Desktop / Windsurf (`mcp.json`)
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

### Agent Skill (`skills.sh`)
```bash
npx -y skills@latest add AbigailDavised/tbmlib-mcp -y
```

## License

MIT © [TbmLib](https://tbmlib.com)
