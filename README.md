
Project - Symphony Text Parser (Windows)
======

Notice
--------
Development of this program is currently on hiatus. Work on this program will commence some time in the future

Project Outline
------
Staff have complained about the Mac version of the Symphony Report to Barcode Program. This app even though made for windows will serve as a guidline for developing the macOS version of this app.

The app should take a report generated by Symphony Workflows and parse through the information within and once done report to the user what its status is and if successful export the data to an excel spreadsheet with propper formatting.

The app will use EPPlus. EPPlus is a community created library which gives C# the ability to generate, read & edit `.xlsx` files. The benefit of using this compared to `Office.Excel.Interop` is that it runs on both macOS and on Windows, another benefit of using `EPPlus` is that it doesn't require that the host machine have Excel installed where `Office.Excel.Interop` does.


How will the Program work?
--------------
Firstly it'll ask for the class that the report will be for. The program will then require the directory that the symphony report is stored in. Once pointed to the directory the program will parse through the data and remove any unnecessary data. It will then move the parsed data to an `.xlsx` document. which would be kept in local storage. `Student IDs` should be written in the font `Free 3 of 9 extended` with an appropriate font size.

If done correctly the program will export an xlsx file that contains all users and their barcodes (Student Id), all of which should be properly spaced appart and easy to read. 
