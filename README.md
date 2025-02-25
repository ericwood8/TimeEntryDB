# TimeEntryDB
This is the MS Sql Server database layer for the TimeEntryUI and TimeEntryServer repos. 

The TimeEntry is a .NET Aspire designed to streamline workforce management.
Its purpose is for employees to be able to:
  1) enter their time for the day
  2) request leave, clearance, expense reimbursement, and overtime

---

## Prerequisites

Before beginning, make sure you have the following tools installed:

1. **Microsoft SQL Server**
    - Download and install MS SQL Server:  https://www.microsoft.com/en-us/sql-server/sql-server-downloads
    - **The free Developer or free Express version is fine**
    - Verify that this is completely functional.
2. Some tool to unzip the zip files.
3. Unzip the two files so there is a MDF and a log file both in the same directory.
     
---

## How To Attach DB

On your local computer using the MS Sql Server Management Studio:
  1) Run "MS SQL Server" as Administrator by doing right-click and choosing option.
  2) Connect by "Connect Object Explorer" using Windows Authentication
  3) Click on "Databases" folder node under your computer name or server name.
  4) Right-click to "Attach..."
  5) If you see nothing, then double-check it is not in the "SQL2022" directory or in folder where connection user does not have permissions.
  6) Click "Add" button and find files TimeEntry.mdf and TimeEntry_log.LDF.
  7) Click "Ok" button.
  8) If "Access is Denied" error then verify that you are in Administrator mode. (See 1 above).
  9) Verify and understand the connection string to this TimeEntry database to use in the TimeEntryServer repo.

Should appear as TimeEntry database.
