# This repository reproduces accuracy issues with Ledger and hledger.

In `ledger.dat` you will find an example ledger.

Both `ledger -f ledger.dat balance -X CHF` and `hledger -f ledger.dat bal
--infer-market-prices -X CHF` show a non-zero balance because the (same) transaction
is incorrectly considered balanced and errors add up.
