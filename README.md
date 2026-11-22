# Alert Simulator Prototype

Prototype of the web-based system for our Fundamentals of Research study, **"Will Metro Manila Adults Act on the Alert? Message Completeness, Language, and Alert Comprehension"** (Group Atlas, BSIT, PUP CCIS). It follows Chapter 3 and Appendix 1 of the paper.

**Live site:** https://sramos06.github.io/alert-simulator-prototype/

## What's in it

- **Survey**: what respondents see. Bilingual consent and screening (18+, Metro Manila), a six-item profile, random assignment to one version in balanced blocks of four, and four alerts in random order on a phone lock screen labeled SIMULATION (closes on OK or after 30 seconds). After each alert: the four-item intention-to-act scale, then the five-item comprehension test. An attention check follows the second alert, and a preference pick is made for each alert type. A browser that already submitted cannot answer again.
- **Alerts**: all 16 alerts (4 alert types × 4 versions) with their elements, plus the four real NDRRMC alerts (Table 1 of the paper) that the typical versions are modeled on.
- **Composer**: for alert writers. Fill in the five elements and it writes a complete alert in Filipino and English, with a character counter, an element check, an approve step, and the language respondents preferred marked as recommended.
- **Checker**: paste any alert to see which of the five elements (hazard, location, time, guidance, source) are missing.
- **Evaluate**: the ISO/IEC 25010 questionnaire for IT experts and DRRM staff.
- **Results**: respondents per version against the target of 46, mean scores by alert type and version, preferences with the language rule, "did not say" rates, evaluation means with interpretation, and CSV exports for JASP.

| | Filipino | English |
|---|---|---|
| **Typical** (no time, no guidance) | A | B |
| **Complete** (all five elements) | C | D |

## Scoring

Comprehension is scored per version: for typical alerts, "The alert did not say" is the correct answer to the time and guidance items. Intention to act is the mean of four 1–5 ratings.

## Prototype limits

- Responses are saved only in the browser you use. The real system saves to Google Sheets through Apps Script, keeps the randomization block count and the answer key there, and opens the dashboard only through the researchers' account.
- Demo respondents are made up so the tables aren't empty. They are not results.
- All alerts are simulated, were not sent by any agency, and still need checking by our validators.
