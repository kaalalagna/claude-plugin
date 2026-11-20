---
name: kaala-lagna
description: Use when the user asks about Vedic astrology, their horoscope or jathagam, Dasa/Bhukti, Panchang, a horoscope PDF, an unknown birth time, or a family member's birth profile, and Kaala Lagna's tools are connected.
---

# Kaala Lagna

Kaala Lagna holds the user's family birth profiles and one shared credit wallet. Use the Kaala Lagna
MCP tools for everything; never guess charts or dates yourself.

## Whose horoscope

1. `list_birth_profiles`, then ask the user which person they mean. Never pick for them.
2. `select_birth_profile` with that profile; keep the returned `selection_id` for questions.
3. If the user mentions someone else, ask again and select that profile.

## Questions (use credits)

- `ask_astrology_question` with the selection. Answers come in English unless the user asks for
  Tamil, Hindi, Telugu, Malayalam or French; for an earlier answer in one of those, use
  `get_reading_in_language`.
- Show the returned `answer` exactly, word for word, including its closing line. Do not summarise,
  restructure or add predictions, timings or advice of your own.
- Mention `credits_charged` and `credits_balance`.

## Free tools

- `get_birth_chart`, `get_dasha_details`, `get_panchang`, `get_horoscope_pdf` (give the link as a
  clickable link; `chart_style` north or south only if asked).
- New person: `search_birth_place`, let the user pick the place, confirm the details, then
  `create_birth_profile`.
- Birth time unknown: ask for the part of the day, then the dates of happy life events (marriage,
  each child's birth, buying a house or land or a vehicle, other joyful events), then
  `find_birth_time`. Only call `apply_birth_time` after the user agrees.
