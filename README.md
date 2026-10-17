# Power BI for Beginners — course files

Free files for the **Power BI for Beginners** video course by [Asan Tutorials](https://www.youtube.com/@AsanTutorials).

> 🚧 The course is in production. Lessons appear here on the day each video goes public.

## How to use these files
1. Install the **latest** Power BI Desktop (older versions can't open newer files).
2. Make a folder called **`PowerBI-Course`** on your C drive: `C:\PowerBI-Course`. The videos use this folder too, so everything you see on screen matches your PC.
3. Download the data (the green **Code → Download ZIP** button), unzip it, and copy the `data` folder into it. You now have `C:\PowerBI-Course\data\contoso\sales.csv`.
4. Each lesson has its own page in `lessons/` (one folder per chapter). Its **Files** table links the Power BI file you need: click the file name, then the **Download raw file** button (the arrow at the top right). Save it in the chapter's folder, for example `C:\PowerBI-Course\ch02\`.
5. A lesson starts from the end file of the lesson before it. Open that file, and follow along. Stuck? Open the lesson's own end file.

> Using another folder? That's OK. The course's Power BI files look for the data in `C:\PowerBI-Course\data`, so the first time you refresh, change the path once: **Transform data → Data source settings → Change Source**.

## What's here
| Folder | What |
|---|---|
| `data/first-report/` | One CSV file with all sales, for the first report (Lesson 1.5) |
| `data/contoso/` | The Contoso sales data (CSV files) |
| `data/messy/` | Messy files for the Power Query lessons |
| `lessons/` | One folder per chapter (for example `lessons/ch01-getting-started/`), with one folder per video inside: link to the video, what you'll learn, the Power BI file (`.pbix`) of the lesson, the "Your turn" challenge and its answer |
| `glossary/` | Every term from the course with a simple definition (PDF) |

## The story
You are the new data analyst at Contoso, a shop that sells electronics in 8 countries and online. Sara, the Sales Manager, has a question: *why did sales fall after 2023?* Lesson by lesson, you build the report that answers it.

## Credits and licenses
- Data: **Contoso Data Generator V2 by SQLBI**, MIT License (see `data/contoso/LICENSE`). https://github.com/sql-bi/Contoso-Data-Generator-V2
- Data: all files in `data/` are under the MIT License (the practice files in `data/first-report/` and `data/messy/` are made from the Contoso data).
- Course files (lesson pages, Power BI files, glossary): **CC BY-NC 4.0** by Asan Tutorials. Free to share and adapt with credit, not for commercial use. See [`LICENSE`](LICENSE).
