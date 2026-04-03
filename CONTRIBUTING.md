# Contributing to Korean Expression API

Thank you for your interest in contributing! This dataset helps Korean learners worldwide understand how expressions are actually used by native speakers.

## How to Contribute

### Add a new expression

1. Fork this repo
2. Add your expression to `expressions.json` following the existing schema
3. Include at minimum: `expression`, `romanization`, `literal`, `real_meanings` (2+), `register`, `frequency`
4. Optional but appreciated: `guide_url`, `search_url`
5. Submit a PR with a brief explanation of why this expression is commonly misunderstood

### Improve existing data

- Fix romanization errors
- Add missing meanings or usage contexts
- Update frequency ratings
- Add register variants (formal/informal/casual)

### Expressions we'd love to see added

- 진짜 (jinjja) — ranges from "really?" to "are you kidding me"
- 아이고 (aigo) — the universal Korean exclamation
- 화이팅 (hwaiting) — encouragement that doesn't translate
- 답답하다 (dapdaphada) — frustrated but not angry
- 치킨 (chikin) — why Koreans say "chicken" differently

## Schema

```json
{
  "expression": "한국어 표현",
  "romanization": "hangugeo pyohyeon",
  "literal": "literal English meaning",
  "real_meanings": ["contextual meaning 1", "contextual meaning 2"],
  "register": "polite/casual/formal/neutral",
  "frequency": "very high/high/medium/low",
  "guide_url": "https://tubelang.com/korean-expressions/en/slug (optional)",
  "search_url": "https://tubelang.com/ko/en/search?q=표현 (optional)"
}
```

## Code of Conduct

Be kind. We're all here to help people learn Korean.
