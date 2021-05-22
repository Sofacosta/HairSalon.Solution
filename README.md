# Hair Salon 💅
## Independent project: Database Basics
### Project initiated: 05-20-2021
### Project modified: 05-21-2021 
### By Sofia Acosta
## Project Description
MVC web application to help a hair salon manage her employees (stylists) and their clients
* The user (hair salon manager) should be able to add a list of stylists
* For each stylist, add clients who see that sytlist
* The stylist have specific specialities, so each client can only see a single stylist

## Technologies Used
 
```
* C#
* .NET
* MySQL | MySQL Workbench
* MSBuild
* Bootstrap
* Razor
* HTML Helper

 ```

## Set up / Installation requirements
* Open the terminal in your machine
* Navigate to the directory where you would like to save this project 
* Clone the project with $ git clone https://github.com/Sofacosta/HairSalon.Solution.git
* Type "dotnet build" in root folder and hit enter
* To start program. navigate to HairSalon and press the dotnet watch run command. 
* Create appsettings.json and add this code into it: {
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=sofia_acosta;uid=root;pwd=[PASSWORD];"
  }
}      
```
Setup Database

CREATE DATABASE 'Firstname_Lastname';
CREATE TABLE `sofia_acosta`.`stylists` (
  `StylistId` INT NOT NULL AUTO_INCREMENT,
  `Name` VARCHAR(45) NULL DEFAULT 0,
  `Description` VARCHAR(45) NULL DEFAULT 0,
  `HireDate` INT NULL DEFAULT 0 AFTER `Description`;
  PRIMARY KEY (`StylistsId`));
CREATE TABLE `sofia_acosta`.`clients` (
  `ClientId` INT NOT NULL AUTO_INCREMENT,
  `ClientName` VARCHAR(45) NULL DEFAULT 0,
  `StylistId` INT UNSIGNED ZEROFILL NULL AFTER `Name`;
  PRIMARY KEY (`ClientId`));
```
![sqlimg](/images/sqlimg.png)

## Known Bugs

## Notes

## License
* [MIT](https://choosealicense.com/licenses/mit)
* Copyright 2021 Sofia Acosta
## Contact
* Sofia Acosta sofiaacostarascon@gmail.com