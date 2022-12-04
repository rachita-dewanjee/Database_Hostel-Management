# Hostel Management System

A desktop application for managing a hostel, built in **Java Swing** (NetBeans) with a
**Microsoft SQL Server** database connected through JDBC.

## Features
- User login and sign-up
- Records for students, rooms, staff, furniture and bills
- Add, update, delete and search for each record type
- Combined views such as student bills, student hostels and room furniture

## Tech
Java (Swing GUI built with the NetBeans form designer), Microsoft SQL Server, JDBC
(`com.microsoft.sqlserver.jdbc.SQLServerDriver`), Apache Ant build (`build.xml`).

## Run it
1. Install SQL Server and create a database named `HOSTELMANAGEMENTSYSTEM` with the tables the app uses
   (`log_in000`, `HOSTEL0`, `ROOM00`, `bill0`, `furniture0`, `staff0`, `student0`).
2. Add the Microsoft JDBC driver for SQL Server (`mssql-jdbc` jar) to the project libraries.
3. In the files under `src/hostelmanagement/`, replace `YOUR_USERNAME` and `YOUR_PASSWORD` in the
   `DriverManager.getConnection(...)` calls with your SQL Server login.
4. Open the project in NetBeans and run `HOSTELMANAGEMENT.java` (or build with `ant`).
