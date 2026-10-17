# Lesson 2.3 — Load Excel and a folder of files

▶️ **Video:** <video link>

Sara sends two new things: her sales targets in an Excel workbook, and a folder with twelve monthly sales files. In this lesson you load the Excel sheet with the Navigator, and you combine the whole folder into one table.

## What you'll learn
- Load an **Excel workbook** and pick a sheet in the **Navigator**
- Load a whole folder with **Get data → More… → File → Folder**
- **Combine files** into one table, and check it with the **Source.Name** column

## Files
| | File | Where |
|---|---|---|
| Start | [`c02v02-end.pbix`](../c02v02-load-csv/c02v02-end.pbix) (customer, product, sales, store) | Download it, and save it in `C:\PowerBI-Course\ch02\` |
| Data | `sales-targets-2025.xlsx` and the folder `monthly-sales` (12 CSV files) | `C:\PowerBI-Course\data\messy\` (see the [main README](../../../README.md)) |
| End | [`c02v03-end.pbix`](c02v03-end.pbix) (adds Targets 2025 and monthly-sales) | Download it, and save it in `C:\PowerBI-Course\ch02\` |

## The steps in short
**Excel**
1. **Home → Get data** (the words "Get data", next to the arrow) → **Excel workbook**.
2. Go to `C:\PowerBI-Course\data\messy`, click **sales-targets-2025**, then **Open**.
3. In the **Navigator**, select the **box** next to **Targets 2025** (clicking the name only shows the preview), then **Load**.

**Folder**
1. **Home → Get data → More…** → **File** → **Folder** → **Connect**.
2. Type the folder path `C:\PowerBI-Course\data\messy\monthly-sales`, then **OK**.
3. Check the file list: twelve files, all `.csv`, nothing else in the folder.
4. Open **Combine** → **Combine & Load**. In the **Combine Files** window, check the **Delimiter** (Comma), then **OK**.
5. **Table view** → **monthly-sales**: the first column, **Source.Name**, shows which file each row came from. The bar at the bottom shows 37,708 rows.

💡 **Good to know:** these monthly files hold the 2025 sales, which are also in the `sales` table. In chapter 3 you learn to put files like these together the right way.

⚠️ **Common mistake:** Power BI combines *every* file in the folder, even in folders inside it. Keep only files with the same column names there.

## Your turn
Open **Targets 2025** in **Table view** and click the arrow next to **Category**. How many categories does Sara have targets for?

<details>
<summary>Answer</summary>

**8 categories**: Audio; Cameras and camcorders; Cell phones; Computers; Games and Toys; Home Appliances; Music, Movies and Audio Books; TV and Video.

The bar at the bottom says the same: 8 rows, one for each category, with a target for each month (Jan to Dec). Press **Escape** to close the list without changing anything. Your file now matches `c02v03-end.pbix`.
</details>

---
Previous: [2.2 Load CSV files](../c02v02-load-csv/) · Next: [2.4 Load vs Transform data, and Refresh](../c02v04-load-vs-transform/)
