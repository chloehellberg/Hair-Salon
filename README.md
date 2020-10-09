# _Eau Claire's Salon Project_

#### _Console application for a hair salon using C#/.NET, MySQL and Entity Framework, Oct 9th 2020_

#### By _**Chloe Hellberg**_

## Description

_This is an MVC web application for a hair salon owner to help manage their employees (stylists) and the clients associated with each stylist. Salon owner should be able to add a list of stylists working at the salon, and for each stylist, add clients who see that stylist. The stylists have specific specialties, so each client can only see/belong to a single stylist._
  * _Functions Available_
    * See list of stylists
    * Select a stylist and see their details including a list of all clients that belong to that stylist
    * Add stylists to the database when they are hired
    * Add new clients to a specific stylist
    * Add an appointment for a client
  

## Setup/Installation Requirements

#### Project Folder Setup
* _Download Option_
  * Download files from GitHub repository by click Code and Download Zip
  * Extract files into a single directory
  * Go into appsettings.json and change the password to match your SQL password if needed
  * Run GitBASH in directory
  * Type "dotnet restore" to get bin and obj files
  * Type "dotnet run" in GitBash to run the program
  * Have fun with Eau Claire's Salon!

* _Cloning Option_
  * For cloning please use the following GitHub [tutorial](https://docs.github.com/en/enterprise/2.16/user/github/creating-cloning-and-archiving-repositories/cloning-a-repository)
  * Place files into a single directory
  * Go into appsettings.json and change the password to match your SQL password if needed
  * Run GitBASH in directory
  * Type "dotnet restore" to get bin and obj files
  * Type "dotnet run" in GitBash to run the program
  * Have fun with Eau Claire's Salon!

#### Production Database Setup

* Setup with SQL Statements
  * Enter the below code into your SQL database to create/run: 

    CREATE DATABASE `chloe_hellberg` /*!40100 DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci */;
    USE `chloe_hellberg`;
    CREATE TABLE `clients` (
      `ClientId` int(11) NOT NULL AUTO_INCREMENT,
      `Description` varchar(255) DEFAULT NULL,
      `StylistId` int(11) DEFAULT '0',
      `Appointment` varchar(255) DEFAULT NULL,
      PRIMARY KEY (`ClientId`)
    ) ENGINE=InnoDB AUTO_INCREMENT=16 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
    CREATE TABLE `stylists` (
      `StylistId` int(11) NOT NULL AUTO_INCREMENT,
      `Name` varchar(255) DEFAULT NULL,
      PRIMARY KEY (`StylistId`)
    ) ENGINE=InnoDB AUTO_INCREMENT=5 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;


## Known Bugs

_The appointment button currently doesn't work. When an appointment is added to a client it deletes that client name from the database._

## Support and contact details

_If you run into issues, please email chloe.hellberg@gmail.com with questions or concerns. Feel free to contribute to this code._

[GitHub](https://github.com/chloehellberg)

## Technologies Used

_Main Programs_
  * C# and .NET
  * MySQL
  * Entity Framework
  * CSS and Bootstrap

### License

*Licensed under MIT*

Copyright (c) 2020 **_Chloe Hellberg_**
