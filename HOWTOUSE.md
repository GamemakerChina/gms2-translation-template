# How to use

Need:
OmegaT  
Microsoft Excel (2010 and later) (Or alternatives, e.g. WPS Office Spreadsheets, LibreOffice Calc)  
Visual Studio Code (You can use other code editors instead. e.g. Notepad3, Sublime Text)  

<details><summary>Extract source from CSV file</summary>
### Step 1: Extract from original file

Use Excel to open `english.xml` from `path\to\GameMaker Studio 2\Languages` folder.

Copy the data in the third column.

![](./screenshots/9.png)

Create a new Excel window and paste the data into the first column:

![](./screenshots/10.png)

### Step 2: Save file

Save as an XML document that can be recognized by OmegaT.

The format recognized by OmegaT is `XML Spreadsheet 2003`, and name it `english.xml`

![](./screenshots/11.png)

Use the same approach for DnD (DnD is in `path\to\GameMaker Studio 2\DnDLibs\YoYo Games\Languages`, but in order to avoid conflicts, you should name it  `english_dnd.xml`

### Step 3: Import XML to OmegaT

Copy `english.xml` and `english_dnd.xml` into OmegaT project's `source` folder.

Reload this project.

</details>

<details><summary>Use Template</summary>

### Step 1: Download

Fork and pull this repository by OmegaT (`Project --> Download Team Project`).

Enter your forked repository URL:

![](./screenshots/1.png)

### Step 2: Change your target language
Go to `Project --> Properties` (Or press `Ctrl+E`), change value in `Translated Files Language` and Press `OK` and reopen the project to apply.

![](./screenshots/2.png)

![](./screenshots/3.png)

### Step 3: Start your work

P.S.: This is my work layout, you can customize your layout.

OmegaT tutorial is inconvenient to explain too much here, if you need help, you can use a search engine(e.g. Google)

![](./screenshots/4.png)

### Step 4: Export translated files

Go to `Project --> Create Translated Documents` (Or press `Ctrl+D`) to generate the translated files. then go to `Project --> Access Project Contents --> Target Files` to find them.

![](./screenshots/5.png)

### Step 5: Apply translated

Copy an original CSV file `english.csv` from GameMaker Studio 2 IDE `Languages` directory (e.g. `C:\Program Files\GameMaker Studio 2-Beta\Languages`).

(DnD is in `C:\Program Files\GameMaker Studio 2-Beta\DnDLibs\YoYo Games\Languages`. To prevent duplication of naming, please rename it to `english_dnd.csv`)

Paste the two files into the directory you prepared (I used to paste them into the target folder of the project)

Open `english.xml` and `english.csv` by Excel, click column A press `Ctrl+C` to copy in `english.xml`， then click column C in `english.csv`  press `Ctrl+V` to paste and overwrite data.

For `english_dnd`, use the same approach.

Finally, save them.

![](./screenshots/6.gif)

### Step 6: Rename files

Rename modified `english.csv` and `english_dnd.csv` to your language name (in English).e.g. `chinese.csv` and `chinese_dnd.csv`

### Step 7: Check the file and remove the extra commas(optional if the extra commas exist)

In the process of making language files, extra commas may appear, which will cause GameMaker Studio 2 to fail to recognize the language files correctly. If you find any, please use the code editor to remove them in batches.

In theory, the number of extra commas in each line is the same, you can easily use the "Find-Replace" function of the code editor to remove the commas.

### Step 8: Apply and test translated files

Copy the produced CSV language files back to the `Language` folder of GameMaker Studio 2 IDE.

![](./screenshots/7.gif)

Open GameMaker Studio 2 IDE, and go to `File --> Preferences --> General Settings --> IDE language`. If the IDE recognizes it correctly, it will be displayed here.

![](./screenshots/8.gif)

</details>

