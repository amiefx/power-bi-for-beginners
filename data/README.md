# Data

Copy this folder to `C:\PowerBI-Course\data` (see the main README). The course videos and the start/end files use that path.

## contoso/
The Contoso sales data, ready-to-use set `csv-100k` from **Contoso Data Generator V2 by SQLBI** (MIT License, see `contoso/LICENSE`).

| File | What one row means |
|---|---|
| sales.csv | One line of an order (about 224,000 lines, May 2016 – December 2025) |
| orders.csv | One order (the header) |
| orderrows.csv | One line of an order (same as sales, without the header columns) |
| customer.csv | One customer (fictional people) |
| product.csv | One product (8 categories) |
| store.csv | One store (73 stores in 8 countries, plus the online store: 74 rows) |
| date.csv | One day (2016–2026) |
| currencyexchange.csv | One exchange rate for one day |

All amounts are in **US dollars**.

The files are saved as UTF-8 with a byte-order mark (BOM), so Power BI reads accented names such as "Franche-Comté" correctly by itself. The data is exactly SQLBI's csv-100k set; only those 3 bytes were added.

## messy/
Files made from the Contoso data for the Power Query lessons (Chapter 2 and 3): a customer list "from the CRM" with errors, one sales file per month for 2025, and a sales-targets file "from finance" with one column per month.
