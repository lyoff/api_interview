# API Challenge

Design and implement a RESTful API that could be used to keep track of product inventory counts and locations. 


# Requirements

The 4 API operations we expect to see would be:

* List all quantities available at a location. Example, 


    for poduct id "abc" return:
    
    ”yerevan” -> 15
    ”gyumri” -> 22


* add inventory operation (support positive and negative change) 

    Example: 
        add Inventory for product “abc” location “gyumri” quantity 7: add 7 in gyumri
        add Inventory for product “abc” location “yerevan” quantity -3: reduce in yerevan by 3i
    
    
* reset Inventory for productId: reset all inventory to 0

* get total inventory for productId: return integer sum of all quantities in all locations



The information the product needs to have is:

* product id
* product name

The API responses must be in JSON.


# Setup

We provide you with a starter Spring Boot project. The project is already configured to use 
Spring MVC and talks to an in memory HSQLDB to store the results. 
Jackson is already included to provide JSON serialization and deserialization.

The Spring Boot Started Test module is included to facilitate both unit and integration tests.

Feel free to pick a different framework if you feel more comfortable doing so.

## Dependencies

This project uses Maven for builds.
You need Java 8 installed.



## Building

```
$ mvn package
```

## Running

You can run the app through Maven:

```
$ mvn spring-boot:run
```

or you can run the jar file from the build:

```
$ java -jar target/api_interview-0.1.0.jar
```

# Duration

You will have until the end of the day to complete the challenge. 
In our tests, we found it to take us about 3 hours to build. 
We encourage you to spend any leftover time to polish/document/test your app. 

Please publish your code to your own github repo and send us a link by email.


Please do not share the details of this challenge with anyone.

## Dependencies

This project uses Maven for builds.
You need Java 8 installed.

## Building

```
$ mvn package
```

## Running

```
$ java -jar target/api_interview-0.1.0.jar
```