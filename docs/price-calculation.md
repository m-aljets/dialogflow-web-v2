# Chat Bot Price Calculation

- basis: [Dialogflow pricing table](https://cloud.google.com/dialogflow/pricing#es-agent)

### Assumptions

- `Dialogflow ES` (Essentials Edition): standard agent type
- midsize company
  - 2500 chat bot requests / month
- audio support
  - input: 10%, each appr. 10 sec long and
  - output: standard voice, appr. 250 presonses per month each around 200 characters
- no `Mega Agent` (< 2000 intents)
- no sentiment analysis

### Calculation

| item | amount (per month) | price ($) | sum ($)|
|------|---------------------|----------|--------|
| requests | 2500            | 0,002     | 5     |
| audio input | 250 * 10 sec | 0,0065 per 15 sec | 1,08 |
| audio output | 250 * 200 chars | 4,00 per mio chars | 0,2 |
| **sum** | | | **6,28** |

