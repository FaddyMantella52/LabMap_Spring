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
  		
