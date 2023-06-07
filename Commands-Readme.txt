* To build your project use command:
             (Project_Folder/dotnet build)
 
	Project Folder :
	Customer Module - Customer/Customer.WebAPI
	FoodMenu Module - FoodMenu/Foodmenu.WebAPI
	Order Module - Order/Order.WebAPI
	API GateWay - OcelotGateway

* On command prompt, cd into your project folder (cd <Your-Project-folder>).

* To connect SQL  server from terminal:
	( Project_Folder /sqlcmd -S localhost -U sa -P pass@word1 )
	
	-To create database from terminal - 
	1> Create Database Database_Name
	2> Go

* Steps to Apply Migration(Code first approach):
	Press Ctrl+C to get back to command prompt
	Run following command to apply migration-
             ( Project_Folder /dotnet-ef database update)

*  To check whether migrations are applied from terminal:
	( Project_Folder /sqlcmd -S localhost -U sa -P pass@word1 )
	1> Use Database_Name
	2> Go
	1> Select * From __EFMigrationsHistory
	2> Go

* To launch your application, Run the following command to run the application:
	( Project_Folder /dotnet run )

To run the test cases in CMD, Run the following command to test the application:

	( Project_Folder /dotnet test --logger "console;verbosity=detailed" )
 (You can run this command multiple times to identify the test case status,and   refactor code  to make maximum test cases passed before final submission).

* To ensure your code is saved and available for later use, remember to use the CTRL+Shift+B command on your code IDE.
   This will push or save the updated contents in the internal git/repository.
   It is also important to use CTRL+Shift+B before the final submission to evaluate the code quality.