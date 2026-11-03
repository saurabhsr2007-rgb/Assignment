Everything is consistent per row, so I’ll apply the changes with openpyxl (keeping the tables, formulas and side summaries intact), then recalculate and verify.

I’ve applied all four changes to Formatting.xlsx. I checked the result by rendering it, and no ##### appears anywhere.

Currency Format, date #####: I widened the OrderDate column so the dates always show, for example 1-Jan-2020.
Currency Format, UnitPrice and TotalPrice:
UnitPrice now uses the Currency format ($1.77).
TotalPrice now uses the Accounting format, with the $ aligned to the left edge ($   58.41).
The two matching total cells beside the table (UnitPrice and TotalPrice) use the same formats.
Number Format: every number from Math to the pecentage column is now a percentage with two decimals (for example 82.91%).
Date Format: the Expiry dates show as 02/Jan/2021, Sat. That format was already on every Expiry cell in your file, so I re-applied it and widened the column so it isn’t cut off.
$ symbol: I used $ because your insurance sheet already uses it. To switch to ₹, change the symbol in Format Cells.
pecentage column: it is the formula =B/C/D/E*100, so as a percentage it shows very large figures such as 17219.83%. That is what percentage format does to those values, and you may want to delete or redo that column.
Everything else: the tables, formulas and totals are unchanged (the quantity total is 15,442 and the total price is 33,325.58).
