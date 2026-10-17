# Lesson 2.5 — Data source settings, parameters and storage modes

▶️ **Video:** <video link>

Sara opened our file on her laptop and the refresh failed. In this lesson you find out why, check your data sources, and make the data folder a **parameter**, so the CSV tables refresh on any PC. You also learn the two main **storage modes**.

## What you'll learn
- Why a refresh fails when the data folder has another name (each table saves the full **path** to its file)
- See your sources in **File → Options and settings → Data source settings**
- Create a **parameter** called `DataFolder` and use it in the four CSV tables
- Change the folder later with **Home → Transform data → Edit parameters**
- **Import** (a copy inside your file, needs a refresh) vs **DirectQuery** (asks the source each time)

## Files
| | File | Where |
|---|---|---|
| Start | [`c02v04-end.pbix`](../c02v04-load-vs-transform/c02v04-end.pbix) (customer, monthly-sales, product, sales, store, Targets 2025) | Download it, and save it in `C:\PowerBI-Course\ch02\` |
| Data | the Contoso CSV files | `C:\PowerBI-Course\data\contoso\` (see the [main README](../../../README.md)) |
| End | [`c02v05-end.pbix`](c02v05-end.pbix) (the same six tables; the four CSV tables use `DataFolder` = `C:\PowerBI-Course\data\contoso\`) | Download it, and save it in `C:\PowerBI-Course\ch02\` |

⚠️ In this lesson you rename the folder `contoso` to `contoso-sara` and back. **If you stop halfway, rename contoso-sara back to contoso.** Later lessons need the folder `C:\PowerBI-Course\data\contoso\`.

💡 Your data is in another folder or on another drive? Open `c02v05-end.pbix`, then **Home → Transform data** (the arrow) **→ Edit parameters**, put your folder in **DataFolder** (keep the `\` at the end), click **OK**, then **Apply changes**.

## The steps in short
**Make the refresh fail (Sara's laptop)**
1. In **File Explorer**, open `C:\PowerBI-Course\data`. Click **contoso**, press **F2**, type `contoso-sara` and press **Enter**.
2. In Power BI: **Home → Refresh**. It fails: Power BI can't find the files. Click **Close**.

**Data source settings**
1. **File → Options and settings → Data source settings**. The CSV paths still point to `contoso`.
2. **Change Source...** fixes one path at a time. **Clear Permissions** removes saved sign-in details (for sources that need a sign-in, like a database). Click **Close**.

**Create the parameter**
1. **Home → Transform data** (the icon). Power Query shows the same error.
2. **Manage Parameters** (the arrow) **→ New Parameter**.
3. **Name:** `DataFolder` · **Required:** selected · **Type:** Text · **Current Value:** `C:\PowerBI-Course\data\contoso-sara\` (end it with a backslash). Click **OK**.

**Use it in the four CSV tables**
1. Click **sales**, then the first step on the right, **Source**.
2. In the bar above the data, select from the first quotation mark up to the last backslash, and type `DataFolder & "`. Press **Enter**. The bar now shows `File.Contents(DataFolder & "sales.csv")`.
3. Do the same for **product**, **customer** and **store**.
4. **Close & Apply**: the tables load from Sara's folder.

**Back to your PC**
1. In File Explorer, rename `contoso-sara` back to `contoso`.
2. **Home → Transform data** (the arrow) **→ Edit parameters**. In **DataFolder**, remove `-sara` but keep the backslash. Click **OK**, then **Apply changes**.

⚠️ **Common mistake:** no backslash at the end of DataFolder. Power BI then looks for `...\contososales.csv`.

**Storage mode**
- **Model view** → click **sales** → **Properties** → **Advanced** → **Storage mode**: **Import**. Leave it as it is.

## Your turn
Check the storage mode of **monthly-sales**. Is it Import too? And why can't it be DirectQuery?

<details>
<summary>Answer</summary>

Click **Model view** on the left, then **monthly-sales** in the **Data** pane. In the **Properties** pane, open **Advanced**: **Storage mode** says **Import**.

It can't be DirectQuery, because monthly-sales comes from a folder of CSV files. A CSV file can't answer questions like a database, and neither the Text/CSV nor the Folder connector offers DirectQuery. Nothing changes in your file; it matches `c02v05-end.pbix`.
</details>

---
Previous: [2.4 Load vs Transform data, and Refresh](../c02v04-load-vs-transform/) · Next: 3.1 Power Query Editor tour
