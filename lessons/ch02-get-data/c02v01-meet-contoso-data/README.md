# Lesson 2.1 — Meet the Contoso data

▶️ **Video:** <video link>

Sara has almost 219 million dollars of sales, spread over eight files. What's inside them, and where does she start? In this lesson you meet the Contoso data that the whole course uses.

## What you'll learn
- Where the eight Contoso files are on your PC
- What a **table**, a **row** and a **column** are
- What one row means in each file
- How **keys** connect tables (and why you never add them up)

## Files
| | File | Where |
|---|---|---|
| Data | the folder `contoso` (eight CSV files and a `LICENSE` file) | `C:\PowerBI-Course\data\contoso\` (see the [main README](../../../README.md)) |
| Start / End | none: this lesson doesn't use Power BI files | — |

## The steps in short
1. In File Explorer, open the `PowerBI-Course` folder on your C drive, then `data`, then `contoso`.
2. You see eight CSV files: sales, orders, orderrows, customer, product, store, date and currencyexchange, plus the `LICENSE` file (you may use this data for free).
3. When you load a file into Power BI, it becomes a **table**: data in rows and columns, like in Excel.
4. In `sales`, one **row** is one line of an order: one product, how many, and the price.
5. A **key** is a column with a unique number for each row. `sales` has the ProductKey, CustomerKey and StoreKey of each sale; the files `product`, `customer` and `store` tell you what those numbers mean.
6. Sales amount = Quantity × NetPrice. All rows together: $218,814,471.71, almost 219 million dollars.

⚠️ **Warning:** keys only connect tables. Never add them up: a total of ProductKey means nothing.

## Your turn
Which column in `sales` points to the store that made the sale? And which file has the store's country?

<details>
<summary>Answer</summary>

The column is **StoreKey**: every row in `sales` has the StoreKey of the store that made the sale.

The file is **store** (`store.csv`): one row is one store, with the same StoreKey and its country in the column **CountryName**.

Example: the sale of product 279 has StoreKey 410, and in `store`, StoreKey 410 is "Contoso Store Fermanagh" in the United Kingdom. Online sales have StoreKey 999999, the "Online store"; its CountryName is "Online".

(The customer's own country is in `customer`, found through CustomerKey. Sara asked about the store.)
</details>

---
Previous: [1.5 Your first report in 10 minutes](../../ch01-getting-started/c01v05-first-report/) · Next: [2.2 Load CSV files](../c02v02-load-csv/)
