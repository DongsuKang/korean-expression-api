# Korean Expression API

Open dataset of common Korean expressions with real meanings, pronunciation, usage notes, and links to native speaker video examples.

## Why?

Korean textbooks teach simplified meanings. This dataset captures how native speakers *actually* use these expressions — including emotional register, social context, and variant forms.

## Data

**[expressions.json](./expressions.json)** — 11 commonly misunderstood Korean expressions, each with:

| Field | Description |
|-------|-------------|
| `expression` | Korean text |
| `romanization` | Romanized pronunciation |
| `literal` | Textbook/literal meaning |
| `real_meanings` | Array of actual contextual meanings |
| `register` | Formality level |
| `frequency` | How commonly used |
| `guide_url` | Full expression guide with video examples |
| `search_url` | Search for this expression in native YouTube clips |

## Quick Start

```bash
curl -s https://raw.githubusercontent.com/DongsuKang/korean-expression-api/main/expressions.json | jq '.expressions[0]'
```

## Example Response

```json
{
  "expression": "괜찮아요",
  "romanization": "gwaenchanayo",
  "literal": "It's okay / I'm fine",
  "real_meanings": [
    "Dismissal: Don't worry about it",
    "Polite refusal: No thank you",
    "Acceptance: That works for me",
    "Suppressed hurt: I'm choosing not to make this a thing"
  ],
  "register": "polite (해요체)",
  "frequency": "very high",
  "guide_url": "https://tubelang.com/korean-expressions/en/gwaenchanayo"
}
```

## Use Cases

- **Language learning apps** — Show contextual meanings instead of flat translations
- **NLP projects** — Korean sentiment/pragmatics training data
- **Browser extensions** — Popup Korean expression explanations
- **Flashcard generators** — Auto-generate cards with real-world usage notes

## Video Context

Each expression links to [Tubelang](https://tubelang.com) where you can see the expression used in real YouTube clips by native speakers — free, no signup required.

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — Free to use with attribution.

## Contributing

PRs welcome! Add expressions following the existing JSON schema.
