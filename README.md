# Alert Simulator Prototype

Prototype of the web-based system for our Fundamentals of Research study, **"Will Metro Manila Adults Act on the Alert? Message Completeness, Language, and Alert Comprehension"** (Group Atlas, BSIT, PUP CCIS).

**Live site:** https://sramos06.github.io/alert-simulator-prototype/

## What's in it

- **Survey**: what respondents see. Consent, an 18+ and Metro Manila check, four alerts on a phone lock screen (flood, extreme heat, earthquake, air quality), questions after each, and a preference pick at the end. Versions are assigned in balanced blocks of four, and questions follow the alert's language.
- **Alerts**: all 16 alerts (4 alert types × 4 versions), tagged with which of the five parts they have.
- **Composer**: for disaster office staff. Fill in the five parts and it writes a complete alert in Filipino and English, with a character counter and a draft-then-approve flow.
- **Checker**: paste any alert to see which of the five parts (hazard, location, time, guidance, source) are missing.
- **Results**: scores by version, an effect preview for completeness and language, preferences, and a CSV export for JASP or jamovi.

| | Filipino | English |
|---|---|---|
| **Typical** (missing parts, like real alerts) | A | B |
| **Complete** (all five parts) | C | D |

## Prototype limits

- Responses are saved only in the browser you use. The real system would save to Google Sheets through Apps Script and assign versions on the server.
- The demo responses are made up so the screens aren't empty. They are not results.
- All alerts are simulated for research and are not from NDRRMC or any agency. The alert texts still need checking by our validators.
