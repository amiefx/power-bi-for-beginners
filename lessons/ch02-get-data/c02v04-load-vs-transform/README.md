# Lesson 2.4 — Load vs Transform data, and Refresh

▶️ **Video:** <video link>

Sara asks two questions: when do I clean data first, and how do I get the newest data? In this lesson you look at the data before you load it, open Power Query, and refresh your tables.

## What you'll learn
- Look at the **data preview** in the **Navigator** before you click **Load**
- Clean data → **Load**. Messy data → **Transform Data** (it opens **Power Query**)
- Open Power Query for the tables you already have (**Home → Transform data**) and close it with **Close & Apply**
- **Refresh** every table with one click, or refresh only one table

## Files
| | File | Where |
|---|---|---|
| Start | [`c02v03-end.pbix`](../c02v03-excel-and-folder/c02v03-end.pbix) (customer, monthly-sales, product, sales, store, Targets 2025) | Download it, and save it in `C:\PowerBI-Course\ch02\` |
| Data | `crm-customers.xlsx` (only looked at, not loaded) | `C:\PowerBI-Course\data\messy\` (see the [main README](../../../README.md)) |
| End | [`c02v04-end.pbix`](c02v04-end.pbix) (the same six tables, refreshed) | Download it, and save it in `C:\PowerBI-Course\ch02\` |

⚠️ If you see a yellow bar that says there are pending changes, click **Apply changes**.

## The steps in short
**Look before you load**
1. **Home → Get data** (the words "Get data", next to the arrow) → **Excel workbook**.
2. Go to `C:\PowerBI-Course\data\messy`, click **crm-customers**, then **Open**.
3. In the **Navigator**, select the **box** next to **Customers**. Look at the **Full Name** column: some names are all in capital letters, some all in small letters.
4. Messy data like this needs **Transform Data**. You clean it in chapter 3, so for now click **Cancel**. Nothing is loaded.

**Power Query**
1. **Home → Transform data** (click the icon on top). Power Query opens in its own window, the same one as **Transform Data** in the Navigator.
2. Left: your tables. Middle: the data of the table you click. Top: the cleaning tools.
3. You changed nothing, so click **Close & Apply**. Power Query closes.

**Refresh**
1. **Home → Refresh** (click the icon on top). A small window shows each table as it loads.
2. **Table view** → **sales**: the bar at the bottom still shows 223,974 rows, because the file didn't change.
3. Point at **sales** in the **Data** pane: Power BI shows when it was last refreshed.
4. To refresh only one table: right-click it in the **Data** pane → **Refresh** → **Data**.

⚠️ **Common mistake:** the file changes, so you load it again. Don't load the same file again: click **Refresh**.

## Your turn
Refresh only **Targets 2025**. How many rows does it have? Did the number change?

<details>
<summary>Answer</summary>

In the **Data** pane (Report view or Table view), right-click **Targets 2025**, point to **Refresh** and choose **Data**. Power BI reads the Excel file `sales-targets-2025.xlsx` again; only this table refreshes.

Then click **Table view** on the left and **Targets 2025** in the **Data** pane. The bar at the bottom says **Table: Targets 2025 (8 rows)**: one row for each product category.

Did the number change? **No**: 8 rows before and after, because the file didn't change. Nothing else changes in your file; it now matches `c02v04-end.pbix`.
</details>

---
Previous: [2.3 Load Excel and a folder of files](../c02v03-excel-and-folder/) · Next: [2.5 Data source settings, parameters and storage modes](../c02v05-parameters-and-storage-modes/)
