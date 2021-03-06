# ai-one Excel-to-Textfile Add-In

This MS Excel Add-In loops through an Excel spreadsheet and creates individual text files for each row of data. The user can specify which columns of data are to be included in each text file as well as the column that contains the name of the text file.

# Installation Instructions

##Prerequisites:
* Excel 2010 (or higher)

##Install Steps:
1.	Download a copy of **ExcelToFile.xlam** to your computer. You can find the latest version of the file in [Releases](https://github.com/KurtAiOne/excel-to-textfile/releases).
2.	Open any MS Excel Workbook.
3.	On the **File Menu**, click **Options**.
4.	In the **Excel Options** window, click **Add-Ins**. Locate the **Manage** drop-down list, select **Excel Add-ins** and click **Go...**
5.	In the **Add-Ins** window, click **Browse**. Locate the **ExcelToFile.xlam** file and select **Open**. Ensure that the checkbox next to **Excel to TextFile Add-In** is selected.
6.	Now click **OK** and the Add-In is installed. You should now see an **Add-Ins** Menu with the **ai-one Excel-To-File Converter** button available for all workbooks.

# Execution Instructions

##Prerequisites:
* Spreadsheet with at least two rows of data.
* One row of data contains the titles for the columns in the spreadsheet (ideally this will be the first row in the spreadsheet, however you will be given the option to select a different row if desired).
* One column of data contains unique identifiers for each row. This column needs to contain unique data as it will be used as the filenames for the generated text files.
* The unique identifier column data should not have any of the following characters in the data: `< > : “ / \ | ? *`

## Execution Steps:
1.	Open a spreadsheet that contains data to be converted to text files.
2.	On the **Add-Ins** Menu, click **ai-one Excel-To-File Converter**.
3.	Follow the instructions in the dialog!

# Uninstall Instructions

1.	Open any MS Excel Workbook.
2.	On the **File** Menu, click **Options**.
3.	In the **Excel Options** window, click **Add-Ins**. Locate the **Manage** drop-down list, select **Excel Add-ins** and click **Go...**
4.	In the **Add-Ins** window, uncheck the checkbox next to **Excel to TextFile Add-In**.
5.	Now click **OK** and the Add-In is uninstalled.

# .XLAM Build Instructions

1.  Clone this repository.
2.	Open any MS Excel Workbook.
3.	On the **Developer** Menu, click **Visual Basic**.
4.  From the **Microsoft Visual Basic for Applications** window, select the **File** Menu and click **Import File**
5.  Select each of the `.cls`, `.frm`, `.bas` files from this repository.
6.  Close the **Microsoft Visual Basic for Applications** window and go back to the open MS Excel Workbook.
7.  On the **File** Menu, click **Save As**.
8.  At the **Save as type** drop-down, select **Excel Add-In (*.xlam)**, enter a **File name** and press **Save**.
9.  An `.xlam` MS Excel Add-In file is now created.