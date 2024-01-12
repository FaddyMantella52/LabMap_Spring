# MAPCasino
# Introduction:
Welcome to our MapCasino project, created by Sabau-Balan Luca and Stoica Andrei. This project is designed to show a simplified casino management app. The project is structured  using Java and the Spring Framework, offering both a Command Line Interface(CLI) and an API for interaction.
# Setup:
To use the MAPCasino project, follow these steps:
   	1. Clone the project repository.
    	2. Open the project in your preferred Java Integrated Development Environment(IDE).
     	3. Build the project using Maven or Gradle.
      	4. Configure the database connection in the application.properties file.
       	5. Run the application and enjoy!
# Entity:
+ Bar: barID, barName, productID, cashierID, customerID
+ Cashier: personID, name, email, salary
+ Casino Manager: personID, name, email, hireDate, salary
+ Customer: personID, name, email, loyaltyPoints, totalSpendings
+ Customer-Slot Record: recordID, personID, slotID
+ Game Table: gameTableID, title, type, capacity, providerID,
+ Person: personID, name, email, status
+ Product: productID, type, price, quantity, barID
+ Provider: providerID, name
+ Slot: slotID, title, providerId

# CLI:
Slot CLI The Slot CLI provides commands to manage slots. Here are the available commands, we'll use the Slot model as an example:

+ add {entity} - Add a new entity <br>
  ```add slot <name> <providerID>```<br>
  ```add provider <title>```<br>
  ```add bar <name> <capacity>```<br>
  ```add table <title> <type> <capacity> <providerID>```<br>
  		
# Examples of CRUD Operation with Postman
1. Create(Post)-Add a new Bar (example) <br>
   Request: <br>
      Method: Post <br>
      Endpoint:```/bar/add-bar```<br>
2. Read(GET)-Retrieve Information about Slot (example) <br>
   Request: <br>
      Method: GET <br>
      Endpoint:```/slot/find-slot```<br>
3. Update(PUT)-Modify Slot Information (example)<br>
   Request: <br>
      Method: PUT <br>
      Endpoint: ```/slot/update-slot```<br>
4. Delete (Delete)- Remove a provider (example) <br>
   Request:<br>
      Method: DELETE <br>
      Endpoint: ```/provider/delete-provider```<br>
   
# Use Cases for MAPCasino Management Project with JPA:
   1. Casino Resource Management: <br>
      Use Case: The casino manager and administrators can efficiently manage and organize the casino's collection of slots, providers and game tables using the CRUD operations provided by the RESTful service.
   2. Management of multiple Casinos: <br>
      Use Case: Bigger companies, with multiple casinos, can use the system to store and keep track of slots and employees for each casino.
   3. Bar Management: <br>
      Use Case: The casino can have a bar, and with the help of the MAPCasino Project they can keep track of the products from the bar and the employees that work there.
   4. Employee and Customer Management: <br>
      Use Case: Casino administrators can keep track of employees and customers(salary, loyalty points etc.).
      
