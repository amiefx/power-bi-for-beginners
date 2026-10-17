# Lesson 2.2 — Load CSV files

▶️ **Video:** <video link>

Sara, the Sales Manager, has four sales files. In this lesson you load them into Power BI as tables, and you check each file before you load it.

## What you'll learn
- Load a CSV file with **Get data → Text/CSV**
- Check the **data preview** before you click **Load**
- Add more files, one at a time

## Files
| | File | Where |
|---|---|---|
| Start | A new, empty report (no file needed) | Open Power BI Desktop → **Blank report** |
| Data | `sales.csv`, `product.csv`, `customer.csv`, `store.csv` | `C:\PowerBI-Course\data\contoso\` (see the [main README](../../../README.md)) |
| End | [`c02v02-end.pbix`](c02v02-end.pbix) (all four tables) | Download it, and save it in `C:\PowerBI-Course\ch02\` |

## The steps in short
1. **Home → Get data** (click the words "Get data", next to the arrow) → **Text/CSV**.
2. Go to `C:\PowerBI-Course\data\contoso`, click **sales**, then **Open**.
3. Check the **data preview**: the column names are on top, and there is one value in each column. If you see one long column, the delimiter is wrong.
4. Click **Load**. The table appears in the **Data** pane, named after the file: **sales**.
5. Do the same for **product**.
6. Click **Table view** on the left, then **sales** in the Data pane. The bar at the bottom shows the number of rows: about 224,000.

💡 **Tip:** watch out for commas inside a value, like `Smith, Anna`. If the value has no quotes around it, it splits into two columns, and the rest of the row moves to the right. Always check the data preview.

## Your turn
Load **customer** and **store** the same way. Check each preview before you click **Load**. Then open **Table view** and pick **store**. How many rows does it have?

<details>
<summary>Answer</summary>

**74 rows**: one for each store (73 stores in 8 countries), and the last one is the **Online store**.

How: **Home → Get data → Text/CSV** → click **customer** → **Open** → check the preview → **Load**. Then the same for **store**. In **Table view**, click **store** in the Data pane: the bar at the bottom says *Table: store (74 rows)*.

Your Data pane now lists **customer, product, sales and store**, the same as `c02v02-end.pbix`.
</details>

---
Previous: [2.1 Meet the Contoso data](../c02v01-meet-contoso-data/) · Next: [2.3 Load Excel and a folder of files](../c02v03-excel-and-folder/)
