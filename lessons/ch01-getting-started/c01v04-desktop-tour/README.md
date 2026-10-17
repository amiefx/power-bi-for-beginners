# Lesson 1.4 — Tour of Power BI Desktop

▶️ **Video:** <video link>

You open Power BI Desktop for the first time and see an empty window. Where do you start? In this lesson you learn the main parts of the window, so nothing looks strange when you build your first report.

## What you'll learn
- The **ribbon**: the bar of tabs and buttons at the top
- The **canvas**: the white area where you place visuals
- The **panes** on the right: **Visualizations**, **Data** and **Filters**
- The **views** on the left: **Report view**, **Table view**, **Model view** and **DAX query view**

## Files
| | File | Where |
|---|---|---|
| Start | none: you start with a blank report | — |
| Report used in the video | [`c01v05-end.pbix`](../c01v05-first-report/c01v05-end.pbix) (the report from lesson 1.5) | Download it, and save it in `C:\PowerBI-Course\ch01\` |
| End | none: this lesson doesn't change any file | — |

## The steps in short
1. Open Power BI Desktop and click **Blank report** on the start screen.
2. **Ribbon:** each tab has its own buttons. **Home** has the buttons you use most (like **Get data**), **Insert** adds things to the page (like a text box), **Modeling** works with the data behind the report, **Design** has the themes, and **View** changes what you see, like which panes are open. Can't find a button? Use the **Search** box at the top.
3. **Canvas and page tabs:** the white page in the middle is where visuals go. The page tabs are at the bottom; the **+** adds a new page.
4. **Visualizations pane:** pick a visual type here. A **field** is a column that you can use in a visual.
5. Open a report with data: **File → Open → Browse this device**, then `C:\PowerBI-Course\ch01\c01v05-end.pbix`.
6. **Data pane:** the list of tables and fields on the right. Click the small arrow next to `contoso-sales` to see its fields.
7. Select a chart: new ribbon tabs appear (**Format**, **Data / Drill**). The **Filters** pane (click its arrow to open it) is where you choose which data a visual or page shows.
8. **Views** (the icons on the left): **Report view** builds report pages, **Table view** shows the rows of a table, **Model view** shows the tables and the lines that connect them, and **DAX query view** is where you test numbers (chapter 5). The last icon, **TMDL View**, is for advanced users.

⚠️ **Common mistake:** older videos say "Data view" and "Fields pane". Today they are **Table view** and the **Data** pane.

## Your turn
Find the view where you see the rows. Then find the tab with the themes. And find the button that adds a new page.

<details>
<summary>Answer</summary>

1. The view where you see the rows: **Table view**, the second icon on the left (under Report view). With `c01v05-end.pbix` open, it shows the rows of `contoso-sales`.
2. The tab with the themes: **Design**, on the ribbon at the top (after Modeling). It shows a list of themes; you don't need to pick one.
3. The button that adds a new page: the **+** at the bottom, right of the page tabs ("Page 1").

Then click **Report view** (the top icon on the left) to go back. Clicked the plus? Then you have a new, empty page. To remove it, right-click its tab and choose **Delete page**. Or keep it: it doesn't change the report.
</details>

---
Previous: [1.3 Install Power BI Desktop](../c01v03-install-desktop/) · Next: [1.5 Your first report in 10 minutes](../c01v05-first-report/)
