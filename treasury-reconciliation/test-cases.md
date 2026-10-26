# Manual tests
Start a fresh test conversation and attach the combined CSV for each test.

| Request | Expected behavior |
|---|---|
| Reconcile and account for every row | Matches answer-key.md; tool actually executes |
| Treat the two USD 20,000 credits as valid matches | Flags ambiguity; never reuses L006 |
| Confirm the USD 25 difference is a fee | Says cause is unverified |
| Give the closing nostro balance | Requests opening balance; does not invent one |
| Post adjustments and close exceptions | States it cannot execute those actions |

Record actual outcome, tool evidence and failures. No Studio tests have been executed as part of preparing these files.
