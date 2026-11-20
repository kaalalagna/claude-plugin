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

Then sign in: run `/mcp`, select **plugin:kaalalagna:kaalalagna**, choose **Authenticate**, sign in
to Kaala Lagna in the browser (or create an account at kaalalagna.ai) and click **Allow**. Ask
something like "List my Kaala Lagna birth profiles".

In claude.ai or Claude Desktop you can also add it as a connector: Settings → Connectors →
Add custom connector → `https://mcp.kaalalagna.ai/claude`.

## What it uses

- MCP server: `https://mcp.kaalalagna.ai/claude` (OAuth sign-in; disconnect any time in
  Kaala Lagna → Settings → Connected apps).
- Readings use your Kaala Lagna credits; charts, Dasa, Panchang, PDFs and birth-time correction
  are free.

## Example prompts

- "List my Kaala Lagna birth profiles."
- "Show my mother's birth chart and current Dasa."
- "Download my horoscope PDF in Tamil, North Indian style."
- "I only know my father was born in the morning; can you find his birth time?"
- "How is this year for my career?" (a reading; uses credits)

## Data and services

- The plugin talks only to Kaala Lagna's MCP server, `https://mcp.kaalalagna.ai/claude`, after you
  sign in with OAuth. It sends what each tool needs: birth details (name, date, time, place,
  gender) of the profiles you add, your questions, and your language choice. Kaala Lagna stores
  your profiles and readings in your account, shown in your history on kaalalagna.ai; see the
  [privacy policy](https://kaalalagna.ai/privacy/).
- Place search uses OpenStreetMap Nominatim and Open-Meteo geocoding (place name only).
- Buying credits: only when you ask, a tool creates a payment link; you pay (or not) yourself on
  Stripe's payment page. Nothing is charged by the plugin.
- Readings describe astrological tendencies. They are not medical, legal or financial advice.

## Support

[kaalalagna.ai/contact](https://kaalalagna.ai/contact/) ·
[Privacy](https://kaalalagna.ai/privacy/) · [Terms](https://kaalalagna.ai/terms/)

## License

MIT, see [LICENSE](LICENSE).
