# Copilot banking use cases
UI-first demos for Microsoft Copilot Studio Standard harness.

## Treasury reconciliation
Start with [the walkthrough](treasury-reconciliation/walkthrough.md).

**Current blocker:** Code interpreter is not visible in the user's trial. The guide now gates execution on inspecting the actual UI; the reconciliation integration is not yet configured or verified. The dataset and answer key are ready.

- Upload **treasury-reconciliation/treasury_reconciliation_demo.csv** in the agent test chat.
- Paste **agent-instructions.txt** into the agent instructions.
- Use **test-prompt.txt** for the first run.
- Keep **answer-key.md** and **test-cases.md** for evaluation; do not upload the answer key.
- Separate **internal_ledger.csv** and **bank_statement.csv** are provided for later experiments. Do not upload them alongside the combined CSV: that would double-count the data.

All records are fictional. No customer data or credentials are included.
This compares supplied movements, not opening/closing balances, and is not a production reconciliation engine.
Studio execution has not been tested in the user's environment. Trial capabilities depend on permissions and available features.

Download everything using GitHub **Code > Download ZIP**.
