# PetStore Application

## 1. How to build and/or deploy the API

First you have to build the application using this command:

    ./gradlew build -Dquarkus.package.type=uber-jar

Then use this command to run the application:

    java -jar build/petstore-runner.jar

Then you can type this URL in the browser and see whether the application is working correctly.

    http://localhost:8080/index.html

##  2. How to run test suite

As I mentioned in the document that submitted to the VLE then open the Postman to test the APIs.

First use below URL to send a GET request to view all the pet's data. After send this request you can see details of five pets.

    http:/localhost:8080/v1/pets/start

Then use below URL to send a POST request to add new pet. All the data that should be added are in the URL as parameters. 6 is pet's ID, 1 is pet's age, Burno is pet's name and Dog is pet's type.

    http:/localhost:8080/v1/pets/addOnePet/6/1/Bruno/Dog

Then use below URL to send a GET request to view only one pet. 1 is pet's ID which wants to see the data.

    http:/localhost:8080/v1/pets/find/1

Then use below URL to send a DELETE request to delete a paticular pet's data. 1 is pet's ID.

    http:/localhost:8080/v1/pets/delete?id=1

Then use below URL to send a PUT request to update details of a paticular pet. All the data that should be update are send through the URL as parameters.

    http:/localhost:8080/v1/pets/update?id=3&name=Simba&age=5&type=Lion

All these APIs run and got the results correctly. Screenshots of the APIs and results are in the document that submitted to the UGVLE.
