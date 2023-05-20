# Hajj-itinerary API
A restful API project using the Vapor framework and Postgres database to manage the information of pilgrims and their Hajj itinerary. RESTful API is a way of accessing and manipulating data stored in a database or other data source. (not the database itself). This project is a great, easy-to-learn example for those who want to learn how to build RESTful APIs. Whether you are a beginner or an experienced developer!

#Features
The project provides the following features:

1- CRUD operations

2- Automatic generation of UUID for each Itinerary and Pilgrim item.

3- Automatic calculation of Age in Pilgrim by Date of Birth.

4- Support for JSON

## Tools 🛠️
### Vapor
A server-side Swift web framework that allows developers to build high-performance web applications and APIs.

### Postman
A popular API development tool used for testing, documenting, and managing APIs.

### Postico
A popular and user-friendly PostgreSQL client for macOS that allows users to manage and interact with PostgreSQL databases using a visual interface.

### Postgres
An open-source relational database management system that provides advanced features and scalability for handling complex data storage and retrieval needs.

## Usage

### 1.Pilgrim
| Column Name	 | Type|
| -------------| ------------- |
| id | 	UUID |
| Name | 	String |
| Gender | 	String |
| PNumber | 	String |
| DOB | 	Date |
| Age | 	Integer |

| Request Method | Route | Action |
| GET | /Pilgrim | Returns a list of all Pilgrim items |
|  POST | /Pilgrim | Creates a new Pilgrim item. |
| DELETE Method | /Pilgrim/:id | Deletes an existing Pilgrim item by ID. |

### 1.Itinerary
| Column Name	 | Type|
| -------------| ------------- |
| id | 	UUID |
| CurrentL | 	String |
| Transport | 	String |
| Type | 	String |
| Dstart | 	Date |
| Dend | 	Integer |
| pilgrim_id | 	UUID |

| Request Method | Route | Action |
| GET | /Itinerary	 |Returns a list of all itinerary items |
|  POST | /Itinerary |Creates a new itinerary item. |
| PUT | /Itinerary/:id	 | Updates an existing itinerary item’s type by ID |
| DELETE | /Itinerary:id | Deletes an existing itinerary item by ID. |

All endpoints support JSON encoding and decoding of each Itinerary and Pilgrim items. To create, delete, or update on itinerary’s type, send a JSON payload in the request body.

Example :

![image](https://github.com/MahaaAlassaf/Hajj-itinerary/assets/85122442/8ede8cca-0147-4442-8871-2c74535b9236)

### Visual Interface
![image](https://github.com/MahaaAlassaf/Hajj-itinerary/assets/85122442/cd34cf65-65e9-4793-8376-6700861bbed5)

![image](https://github.com/MahaaAlassaf/Hajj-itinerary/assets/85122442/c951d46c-5a86-4409-bc77-484ba5dc2b1a)


 		
		
		
		


	
	
	
	
	
