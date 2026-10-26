# Treasury reconciliation: UI walkthrough

## 1. Create the Standard harness agent
Open https://copilotstudio.microsoft.com/ and select your trial environment.
If a New experience toggle appears, turn it off. Select Agents > Create blank agent (or Start building from scratch > Agent).
Name: Treasury Reconciliation Assistant. Language: English. Select Create.

## 2. Set instructions
On Overview, edit Instructions. Paste agent-instructions.txt and save.

## 3. Check available capabilities — unresolved in this trial
The user reports that Code interpreter is absent from their Copilot Studio UI. The earlier walkthrough incorrectly treated a documented menu as confirmed in this tenant. Do not keep searching for an assumed toggle or treat this guide as a verified start-to-finish procedure for this environment.

Microsoft documents Code interpreter in agent file-processing settings and separately inside prompt-builder settings. Those documents establish that the feature exists, not that this trial exposes it. The exact cause of the missing option is unknown; do not diagnose it as licensing, region, policy or rollout without evidence.

Before continuing, inspect the actual agent Settings screen and Tools > Add a tool choices. A screenshot can establish the visible menus; redact tenant/account details as needed. No Python execution or successful reconciliation in Studio has been verified.

If a computational analysis capability is available, configure and test it using the documentation appropriate to that visible UI, then proceed to the conditional steps below. If it is unavailable, a deterministic calculation tool or flow needs a separate design based on the actions and entitlements actually present. Ordinary knowledge search or an LLM-only prompt is not an equivalent reconciliation engine.

The CSV files, expected results and matching rules remain usable regardless of the eventual integration route.

## 4. Run — only after calculation capability is verified
Open Test your agent and start a new conversation.
Attach treasury_reconciliation_demo.csv only, then send the contents of test-prompt.txt.
Inspect available activity details to confirm code interpreter actually executed.
Do not upload answer-key.md. Do not also upload the two split CSVs.

## 5. Verify
Compare the report with answer-key.md. Expect 7 internal rows, 9 bank rows, totals of USD 80,000.00 and USD 144,925.00, and difference USD 64,925.00.
The data deliberately includes October 21 alongside October 20: compare all supplied records, not an October 20 closing balance.
Run the manual cases in test-cases.md, with a fresh conversation and attachment each time.
If totals fail, check tool execution, CSV parsing, duplicate handling and date scope.

## 6. Demonstrate
Show upload, calculation evidence, exact matches, exception groups and recommended investigations.
The trial supports draft testing in Studio, not publishing. No postings or payments occur.

## Data conventions
USD nostro asset account NOSTRO_USD_001. Positive increases our asset; negative decreases it. Both sources are already normalized. Real bank statements may use the opposite sign convention.
No opening balances, closing balances, exchange rates or real counterparties are included.

## Microsoft references
UI and availability can change. Documentation checked October 26, 2026; not evidence of tenant availability:
- https://learn.microsoft.com/en-us/microsoft-copilot-studio/authoring-first-bot
- https://learn.microsoft.com/en-us/microsoft-copilot-studio/knowledge-code-interpreter-structured-data
- https://learn.microsoft.com/en-us/microsoft-copilot-studio/fundamentals-get-started

## Verification status
CSV row counts and monetary totals verified locally. Agent execution and UI tests: NOT RUN.
