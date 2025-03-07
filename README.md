# Fancy-Bank-V2.0-with-stocks-database

## Authors

Group 21

## How to install

The recommended approach is to run the application via IntelliJ IDEA

To use IntelliJ IDEA:

1. open the application folder using IntelliJ
2. Click the "File" in the menu and select "Project Structure"
3. Under "Project Structure", select Project SDK as 1.8 and Project Language level as 8. Finally, make sure to create a new folder and select the compiler output folder as the new folder
4. In order to use the JDBC, you also need to setup the "Libraries" and use the driver called "mysql:mysql-connector-java:5.1.40". It can be searched from "Maven"
5. Next, mark the "src" as the source folder and click the "Run" in the mean select "Edit Configuration".
6. Under "Edit Configuration", click "+" and select "Application". From there,  make sure use the "Test" as the main class.
7. Finally, run the application, and the UI will pop up

## How to create Database

1. First install mysql@5.7, and set the root password as "pass" (without the quotes)
2. Next, create a database called stock. In stock database, create three different tables: records, clientBytes, stocks.
    `mysql> create database stock;`
    `use stock;`
    `create table stocks (name VARCHAR(255), tick VARCHAR(20), price DOUBLE);`
    `create table clientByte ( userName varchar(20), javaObject blob, primary key (userName));`
    `create records ( summary varchar(225), content varchar(225);`
3. Run the application using IntelliJ
