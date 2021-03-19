<p align="center"> Authored by Brian Sturgis</p>
<p align="center">Updated on March 12th, 2021</p>

## Detailed Description
This is an MVC web application to help manage employees (stylists) and their clients. The User should be able to add a list of stylists working at the salon, and for each stylist, add clients who see that stylist. The stylists have specific specialties, so each client can only see (belong to) a single stylist.  This is an assignment due to the Epicodus program in March of 2021.

## Objectives (ass quoted from the assignment)
- As the salon owner, I need to be able to see a list of all stylists.
- As the salon owner, I need to be able to select a stylist, see their details, and see a list of all clients that belong to that stylist.
- As the salon owner, I need to add new stylists to our system when they are hired.
- As the salon owner, I need to be able to add new clients to a specific stylist. I should not be able to add a client if no stylists have been added.

## KNOWN BUGS
- the repo name is meant to end in .Solution and the word is spelled .solution.

# Setup/Installation Requirements .Net Installation

## GIT HUB
- repository location (https://github.com/BrianSturgis/JanWeek9Project.solution
- open through a git terminal or clone editor.
- got to repo location.
- using git commands clone to local repo or click "download" and unpack on machine

## Setup and Installation Requirements

### Prior to Installation
* Confirm you have installed .NET installed - this will provide access to the C# language
  * [.NET for macOS](https://dotnet.microsoft.com/download/dotnet/thank-you/sdk-5.0.100-macos-x64-installer)
  * [.NET for Windows](https://dotnet.microsoft.com/download/dotnet/thank-you/sdk-5.0.102-windows-x64-installer)
* Additionally, you may want to install a REPL to allow you to practice, test, and experiment with C#. Below are instructions for the ```dotnet script``` REPL:
  * Install ```dotnet script``` by running the following terminal command: ```$ dotnet tool install -g dotnet-script```
  * **NOTE:** If you just installed .NET 5, restart the terminal. (Otherwise, you will not be able to run the following command.)
    * Enter ```$ dotnet script``` in your terminal and a prompt will open: ```>```
    * To exit the REPL press: Ctrl +C

### Installation
* Clone the repository with the following git terminal command: ```$ git clone https://github.com/BrianSturgis/JanWeek9Project.Solution.git```
* Open the project directory in your terminal
* Navigate to the ```HairSalon``` directory
    * To create ```obj``` directories in both production and test projects, run the terminal command: ```$ dotnet restore```
    * **NOTE**: Do not touch the code in either ```obj``` directory.
* To launch the program, run the terminal command: ```dotnet run```

### Data Base set up
- Confirm you have MySQL installed.
- Confirm you have MySQL Workbench installed.
- Open MySQL Workbench and select Local Instance 3306.
- In the Administration tab, select Data Import/Restore.
- Select Import from Self-Contained File.
- Select the file brian_sturgis.sql from the JanWeek9Project.Solutions root directory.
- Select New from the Default Schema to be Imported To section.
- Choose a name for the database and select Ok.
- Select Start Import.

### MySQL Password Protection
- Create a the following file: appsettings.json in production file root "HairSalon".
- Add the following code: see snippet below
```CS
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=[YOUR_DATABASE];uid=root;pwd=[YOUR_PASSWORD];"
  }
}
```
- [YOUR_DATABASE] must match the database name you chose to import above.
- [YOUR_PASSWORD] must match your local MySQL server password.
- The appsettings.json file is to be included in the .gitignore file.

## Support and contact details
email Brian Sturgis @ <sturujisu@gmail.com>

## Technologies Used
* C#
* NET
* VisualStudio Code
* Git
* GitHub
* MSTest
* coffee
* .NET 5
* ASP.NET Core
* Entity Framework
* MySQL Workbench 8.0.15

### License
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE..

Copyright (c) 2020 **Brian Micheal Sturgis**