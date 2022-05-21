# Salon Management Portal

#### By **Cameron Ray**

#### A client stylist management portal for Eau Claire's Salon

## Technologies Used

* C#
* ASP.Net Core MVC
* Entity Framework
* MySQL

## Description

The "Salon Management Portal" is an online portal for Salons to manage their Employees and clients. Salon owners can track which clients belong to which stylist as well as all of a stylists clients. Owners can update stylist and client information and drill deeper into the client and stylist information.

## Setup/Installation Requirements

* Requires MySQL for the database
* Clone the repository
* navigat to HairSalon.Solution
* Create an appsettings.json file in the root of the HairSalon folder.
```
$ cd HairSalon/
$ touch appsettings.json
```
* Add the following to the appsettings.json file with the bracketed username and password replaced with your mysql username and password.
```
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=cameron_ray;uid=[username];pwd=[password];"
  }
}
```
* restore and build the project
```
$ dotnet restore
$ dotnet build
```
* import the database located in the root of HairSalon.Solution using MySQL Workbench. 
1. From the Navigator section click the Administration tab at the bottom of the section.
2. Click Data Import/Restore and select "Import from Self-Contained File."
3. select the path to import from. In this case it should be the clonedlocation/HairSalon.Solution/cameron_ray.sql
* start the project fomr the HairSalon directory using
```
$ dotnet run
```

## Known Bugs
* missing delete functionality of CRUD

## License

[MIT](LICENSE)

Copyright (c) May 2022 Cameron Ray