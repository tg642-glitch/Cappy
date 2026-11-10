# Tests

`accuracy-results.csv` is the output of CAPPY's in-app accuracy check. The
check runs 20 fictional test invoices through the agents and scores each
answer against an answer key. The CSV has one row per invoice, with:

- the expected answer from the key
- the agents' answer
- whether the verdict, amount and article labels matched
- the agents' reasoning and any open caveats

The last row is the overall score.

## About the answer key

The answer key is the authors' own. It was drafted with Claude and checked
against the FIA PDF by the authors. It covers only 20 invoices, so treat the
result as a smoke test, not a benchmark.

## Results vary

The check calls Claude live, so answers vary between runs. In particular,
which lines get escalated to a human can change from one run to the next.
This file records one run.
