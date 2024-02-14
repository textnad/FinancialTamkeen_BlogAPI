# FinancialTamkeen_BlogAPI
This ApI Created using Asp.Net core 6.
It was designed using Repostrypattern.
* prerequets to run the API:
  - .Net core 6
  - Visual studio 2022.
  - SQl Server.
* To run this API:
  1. Install the Fllowing from nuget package:
     - EntityFrameWorkcore.
     - EntityFrameworkcore.SqlServer.
     - EntityFrameWorkcore.Tools.
  2. Configure your database like following:
     1. Create DB called Employee in SQLSERVER.
     2. In appsetting.json file add the following code:
        ![image](https://github.com/textnad/FinancialTamkeen_BlogAPI/assets/160001814/269a9abd-7c49-4a49-a46f-3bca157fbbc9)
     3. Add the services to the program.cs file:
        ![image](https://github.com/textnad/FinancialTamkeen_BlogAPI/assets/160001814/bcb49044-08d4-4de4-b7e7-65ee0e733fc7)
     4. In nuget package console run the following commands:
        - Add-Migration {name of Migration}.
        - update-database.
    3. Now run the API using swagger in vs2022 OR Postman.
       If you using Postman, follow the following steps:
       1. Create New HTTP project.
       2. Navigate to the URL "https://localhost:{your port number}/" (you can find port number in the file lunchSettings.json)
       3. Choose the HTTP Method you want to test.
         ** For Method Get:**
          - Get All employees: https://localhost:{Your port number}/api/Employee
          - Get one employee: https://localhost:{your port number}/api/Employee/{id}
          **For Post method:**
          https://localhost:{your port number}/api/Employee (do not forget here to choose raw then json and write the record that you                would like to add)
          **For put method:**
          https://localhost:{your port number}/api/Employee/employeeid?id={id}
          and follow the steps in post method
        
