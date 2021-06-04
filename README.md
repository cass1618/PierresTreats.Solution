# Pierre's Sweet & Savory Treats
By Cassandra Copp

## Description
This MVC web application allows the user to add Treats and Flavors to the database. There exists a many-to-many relationship between Treats and Flavors. This app also includes user authentication which prevents a user who is not logged in from make changes.  

## Technologies Used

* C#
* ASP.NET Core
* Entity Framework
* MySQL

### System Requirements 
1. [.NET 5.0](https://dotnet.microsoft.com/download)  
1. [MySQL Community Server](https://dev.mysql.com/downloads/file/?id=484914)
1. [MySQL Workbench](https://dev.mysql.com/downloads/file/?id=484391) (optional, can be used to view and edit the database outside of the application)

### Installation
1. Clone the [PierresTreats.Solution](https://github.com/cass1618/PierresTreats.Solution) Repository

    ### Set Up Required Database
    1. To update the database, dotnet-ef must be installed.  Run the following command in terminal, in any directory:
    ```sh
    dotnet tool install --global dotnet-ef
    ```
    2. To create the database, run the following command in the PierresTreats.Solution/PierresTreats directory:
    ```sh
    dotnet ef database update
    ```
    3. If you would like to view the database you may do so in MySQL Workbench.  The database will be titled cassandra_copp (or whatever the database name in appsettings.json)

2. Add an `appsettings.json` file to the `PierresTreats.Solution/PierresTreats` directory and add the following:
```json
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=pierres_treats;uid=root;pwd=YourPassword;"
  }
}
```
3. Replace YourPassword with your own MySQL password
4. To run the app in terminal, navigate to `PierresTreats.Solution/PierresTreats` directory and enter the command:
```cs
$ dotnet run
```
6. If the server does not automatically open enter localhost:5000 in the address bar of your web browser

## Known bugs

This application has no known bugs.

## License

[MIT](https://opensource.org/licenses/MIT)

Copywrite (c) Cassandra Copp 2021.

## Contact Information

[github.com/cass1618](http://github.com/cass1618)