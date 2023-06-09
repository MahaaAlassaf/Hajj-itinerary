# Hajj-itinerary API
A restful API project using the Vapor framework and Postgres database to manage the information of pilgrims and their Hajj itinerary.
RESTful API is a way of accessing and manipulating data stored in a database or other data source. (not the database itself). This project is a great, easy-to-learn example for those who want to learn how to build RESTful APIs. Whether you are a beginner or an experienced developer!

## Features
The project provides the following features:

1-	CRUD operations

2-	Automatic generation of UUID for each Itinerary and Pilgrim item.

3-	Automatic calculation of Age in Pilgrim by Date of Birth.

4-	Support for JSON


## Tools 🛠️

Download the following:

### Vapor  

A server-side Swift web framework that allows developers to build high-performance web applications and APIs.

### Postman

A popular API development tool used for testing, documenting, and managing APIs.

### Postico 

A popular and user-friendly PostgreSQL client for macOS that allows users to manage and interact with PostgreSQL databases using a visual interface.

### Postgres

An open-source relational database management system that provides advanced features and scalability for handling complex data storage and retrieval needs.

## Requirements

You will need Swift 5.2+


## Usage
The project provides the following tables and their endpoints:

### 1: Pilgrim

| Column Name   |     Type    |
| ------------- | ----------- | 
| `id`          | `UUID`      | 
| `Name`        | `String`    | 
| `Gender`      | `String`    | 
| `PNumber`     | `String`    | 
| `DOB`         | `Date`      |  
| `Age`         | `Integer`   | 

- Where `id` is the `PRIMARY KEY` 

| Request Method |    Route      | Action                                  |
| -------------  | ------------- | -------------                           |
| GET            | /Pilgrim      | Returns a list of all Pilgrim items     |
| POST           | /pilgrim      | Creates a new Pilgrim item.             |
| DELETE         | /Pilgrim/:id  | Deletes an existing Pilgrim item by ID. |


### 2: Itinerary


| Column Name   |     Type    |
| ------------- | ----------- | 
| `id`          | `UUID`      | 
| `CurrentL`    | `String`    | 
| `Transport`   | `String`    | 
| `Type`        | `String`    | 
| `Dstart`      | `Date`      |  
| `Dend`        | `Date`      | 
| `pilgrim_id`  | `UUID`      |

- Where `id` is the `PRIMARY KEY` , and `pilgrim_id` is a `FOREIGN KEY`

| Request Method| Route         | Action                                         |
| ------------- | ------------- | -------------                                  |
| GET           | /Itinerary    | Returns a list of all itinerary items          |
| POST          | /Itinerary    | Creates a new itinerary item.                  |
| PUT           | /Itinerary/:id| Updates an existing itinerary item’s type by ID|
| DELETE        | /Itinerary:id | Deletes an existing itinerary item by ID.      |


All endpoints support JSON encoding and decoding of each Itinerary and Pilgrim items. 
To create, delete, or update on itinerary’s type, send a JSON payload in the request body.

Example : 

<img width="920" alt="Screenshot 1444-08-30 at 2 16 23 PM" src="https://user-images.githubusercontent.com/105675970/226888285-81193234-e1d6-488e-90bb-486e4c823d1b.png">

## Visual Interface 

<img width="1101" alt="Screenshot 1444-08-30 at 2 21 19 PM" src="https://user-images.githubusercontent.com/105675970/226889724-cc3f2816-3545-4866-9de5-b7b25cf0ca35.png">


<img width="1098" alt="Screenshot 1444-08-30 at 2 21 31 PM" src="https://user-images.githubusercontent.com/105675970/226889730-2c6d7f1e-5f34-40d1-86b8-e02a6dd9dc37.png">

## Credits

The project was created by:

Noura Althemali

Maha Alassaf 

Ahod Alshanwah


@2023







