# Steps to Set Up Oracle Client (works with Oracle Instant Client as well) Connection with ODBC driver and Access Data from Excel<br>

## Step 1: Download Oracle Instant Client Files
* Download the following files from the Oracle Instant Client downloads page:
* instantclient-basic-windows.x64-19.24.0.0.0dbru.zip
* instantclient-odbc-windows.x64-19.24.0.0.0dbru.zip

## Step 2: Create Installation Folder
* Create a new folder in the C: drive and name it oracle.
* Inside the C:\oracle folder, unzip both downloaded files. You should now have two folders:
   * C:\oracle\instantclient-basic-windows.x64-19.24.0.0.0dbru
   * C:\oracle\instantclient-odbc-windows.x64-19.24.0.0.0dbru

## Step 3: Consolidate Files
* Go to C:\oracle\instantclient-odbc-windows.x64-19.24.0.0.0dbru\instantclient_19_24.
* Copy all files in this folder.
* Paste them into C:\oracle\instantclient-basic-windows.x64-19.24.0.0.0dbru\instantclient_19_24 to have all necessary files in one location.

## Step 4: Create the TNSNAMES.ORA File
1-In the C:\oracle\instantclient-basic-windows.x64-19.24.0.0.0dbru\instantclient_19_24 folder, create a new file named tnsnames.ora.
2-Replace YOUR_DB_ALIAS with a name for this connection (e.g., ORCL).
3-Replace your_db_host, your_db_port, and your_service_name with the appropriate values for your database connection.
![Added Image](./ODBC-driver-setup-screenshots/Screenshot-2024-11-06-135119.png)<br>

## Step 5: Set Up Environment Variables
1-Add ORACLE_HOME:
   * Click on New under System variables.
   * Set Variable Name to ORACLE_HOME.
   	* Set Variable Value to C:\oracle\instantclient-basic-windows.x64-19.24.0.0.0dbru\instantclient_19_24.
    * Click OK.