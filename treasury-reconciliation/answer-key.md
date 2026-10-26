# Answer key — evaluator only
Do not upload this answer key to the agent.

| Check | Expected |
|---|---|
| Internal rows | 7 |
| Bank rows | 9 |
| Internal movement | USD 80,000.00 |
| Bank movement | USD 144,925.00 |
| Bank minus internal | USD 64,925.00 |
| Exact matches | L001/B001; L002/B002; L003/B003 |
| Amount mismatch | L004/B004; bank minus internal = -25.00 |
| Value-date difference | L005/B005; October 20 versus October 21 |
| Suspected duplicate group | L006, B006, B007; net difference +20,000.00 |
| Internal-only | L007; contributes +15,000.00 to bank minus internal |
| Bank-only charge | B008; contributes -50.00 |
| Bank-only receipt | B009; contributes +30,000.00 |

Difference bridge: -25 + 20,000 + 15,000 - 50 + 30,000 = 64,925.
The value-date difference contributes zero when comparing all supplied records.
Row accounting: 6 exact-match rows + 2 amount-mismatch rows + 2 date-difference rows + 3 duplicate-group rows + 1 internal-only row + 2 bank-only rows = 16.
The USD 25 cause is unverified; do not assume a fee. Duplicate status requires investigation.
These are expected results, not evidence of a Copilot Studio test run.
