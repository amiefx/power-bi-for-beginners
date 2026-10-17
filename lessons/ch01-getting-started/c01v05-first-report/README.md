# Lesson 1.5 — Your first report in 10 minutes

▶️ **Video:** <video link>

Sara, the Sales Manager at Contoso, asks: "How much did we sell? And in which category?" In about ten minutes you load one CSV file into Power BI and build a small report that answers her.

## What you'll learn
- What a **CSV** file is, and how to load it with **Get data → Text/CSV** and **Load**
- What a **field** is, and where to find it (the **Data** pane)
- How to build a **visual**: the same three steps every time
- How to make the page look good: clear names, a title and a theme
- How to save your report

## Files
| | File | Where |
|---|---|---|
| Data | `contoso-sales.csv` (one CSV file, about 224,000 sales) | `C:\PowerBI-Course\data\first-report\` (in this repo: [`data/first-report/`](../../../data/first-report/); setup: see the [main README](../../../README.md)) |
| Start | none: you start with a blank report | — |
| End | [`c01v05-end.pbix`](c01v05-end.pbix) (the three visuals, the title and the theme of the video) | Download it, and save it in `C:\PowerBI-Course\ch01\` |

## The steps in short
1. Open Power BI Desktop and start a **blank report**.
2. On the **Home** tab, click **Get data → Text/CSV**. Open `data`, then `first-report`, pick `contoso-sales` and click **Open**.
3. Look before you load: the first line has the names, and each line below is one sale. Click **Load**.
4. In the **Data** pane on the right, click the small arrow next to `contoso-sales` to see its **fields**.
5. Build a visual, always the same way: **click an empty spot** on the canvas → pick a visual type in the **Visualizations** pane → tick the fields in the **Data** pane.
   - **Card** with Sales Amount: 218.81M, almost 219 million dollars.
   - **Clustered column chart** with Category and Sales Amount: Computers sold the most.
   - **Clustered bar chart** with Customer Country and Sales Amount: customers in the United States bought the most.
6. Clear names: select a visual, double-click its field ("Sum of Sales Amount") under the visual types, type a new name ("Total Sales" for the card, "Sales" for the charts) and press Enter.
7. A title: **Home → Text box**, type "Contoso Sales", press Enter, type "Sales overview". Make the first line big and bold, the second line smaller.
8. A theme: **Design** tab → pick one (the video uses **Frontier**).
9. Save: **File → Save as → Browse this device**, file name `C:\PowerBI-Course\my-first-report`, Enter.

⚠️ **Common mistake:** a visual is still selected when you tick a new field. Then the field goes into that visual. Click an empty spot on the canvas first.

## Your turn
Which customer country bought the most **items**? ("Quantity" is the number of items in each sale.) Build a Clustered bar chart with Customer Country and Quantity. Is it the same country as before?

<details>
<summary>Answer</summary>

Click an empty spot on the canvas first, so no visual is selected (your page is full now: use the free space to the right of the title). Click **Clustered bar chart**, then tick **Customer Country** and **Quantity**.

The longest bar is the **United States**: its customers bought 356,346 items. That's the same country as for Sales Amount. Germany is second with 80,982 items.

The new chart may land small or on top of another visual: drag its corner to make it bigger. Want a clearer title? Double-click "Sum of Quantity" in the field box, type "Items" and press Enter.

Ticked Quantity while another visual was selected? Press Ctrl+Z, click an empty spot, and try again. (This chart is not in `c01v05-end.pbix`.)
</details>

---
Previous: [1.4 Tour of Power BI Desktop](../c01v04-desktop-tour/) · Next: [2.1 Meet the Contoso data](../../ch02-get-data/c02v01-meet-contoso-data/)
