# Kaala Lagna for Claude

Vedic astrology by [Kaala Lagna](https://kaalalagna.ai) in Claude: your family's birth charts,
Dasa/Bhukti, Panchang, horoscope PDFs (South or North Indian charts), birth-time correction from
life events, and personal readings from Kaala Lagna's astrologer in Tamil, English, Hindi, Telugu,
Malayalam and French.

## Install

In Claude Code:

```
/plugin marketplace add kaalalagna/claude-plugin
/plugin install kaalalagna@kaalalagna
```

Then ask something like "List my Kaala Lagna birth profiles". Claude opens the Kaala Lagna sign-in
page; sign in (or create an account at kaalalagna.ai) and approve the connection.

In claude.ai or Claude Desktop you can also add it as a connector: Settings → Connectors →
Add custom connector → `https://mcp.kaalalagna.ai/claude`.

## What it uses

- MCP server: `https://mcp.kaalalagna.ai/claude` (OAuth sign-in; disconnect any time in
  Kaala Lagna → Settings → Connected apps).
- Readings use your Kaala Lagna credits; charts, Dasa, Panchang, PDFs and birth-time correction
  are free.

## Support

[kaalalagna.ai/contact](https://kaalalagna.ai/contact/) ·
[Privacy](https://kaalalagna.ai/privacy/) · [Terms](https://kaalalagna.ai/terms/)

## License

MIT, see [LICENSE](LICENSE).
