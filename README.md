Notes
VBA:
    lastrow = Cells(Rows.Count, 1).End(xlUp).Row
    'Find the last non-blank cell in column A(1)
      lRow = Cells(Rows.Count, 1).End(xlUp).Row
https://www.excelcampus.com/vba/find-last-row-column-cell/      
      'Find the last non-blank cell in row 1
      lCol = Cells(1, Columns.Count).End(xlToLeft).Column
      The Rows.Count statement returns a count of all the rows in the worksheet.  Therefore, we are basically specifying the last cell in column A of the sheet (cell A1048567), and going up until we find the first non-blank cell.

      It works the same with finding the last column.  It starts at the last column in a row, then goes to the left until the last non-blank cell is found in the column.  Columns.Count returns the total number of columns in the sheet.  So we start at the last column and go left.
      .row/column returns the number of the row/column
      The argument for the End method specifies which direction to go.  The options are: xlDown, xlUp, xlToLeft, xlToRight.
subtotal formula in excek not using data tab
https://exceljet.net/excel-functions/excel-subtotal-function
colorindex
  Range("c2").Font.ColorIndex = 5
  Range("c2").Interior.ColorIndex = 4
Python
    if you use double quatation in the print statement to reference a dic, you use single for printing
    print(f'{dic["key"]})
    csv:
    import os
    import csv

    cereal_csv = os.path.join("..", "Resources", "cereal_bonus.csv")
    with open(cereal_csv) as csvfile:
        csv_reader = csv.reader(csvfile,delimiter=",")
        # read the header row first
        csv_header = next(csv_reader)
        print(f"Header: {csv_header}")
GitHub
#clone the repo to local 
git clone url
# made changes to repo
#see the changes 
git status 
#add to the staging stage
git add .
git status # to check if green
# save the change
git commit -m "this is where you type your description"
# push the change to branch
git push orgin master # git push + branch name
