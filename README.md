# Spring Boot E-Commerce Category API

## Overview

This project is a simple **REST API** built with **Spring Boot** for managing product categories in an e-commerce system.
It provides endpoints to create, retrieve, update, and delete categories using a layered architecture.

The application follows a typical Spring Boot structure:

* **Controller layer** – handles HTTP requests
* **Service layer** – contains business logic
* **Repository layer** – communicates with the database using Spring Data JPA
* **Entity layer** – represents database tables

---

## Tech Stack

* Java
* Spring Boot
* Spring Web
* Spring Data JPA
* Jakarta Persistence
* Maven / Gradle
* REST API architecture



### Get All Categories

```
GET /api/public/categories
```

Response:

```
200 OK
```

Returns a list of all categories.

---

### Create Category

```
POST /api/public/categories
```

Request Body:

```json
{
  "categoryName": "Electronics"
}
```

Response:

```
201 Created
```

---

### Update Category

```
PUT /api/public/categories/{categoryId}
```

Request Body:

```json
{
  "categoryName": "Updated Category"
}
```

Response:

```
200 OK
```

---

### Delete Category

```
DELETE /api/public/categories/{categoryId}
```

Response:

```
200 OK
```

---


## How to Run the Project

1. Clone the repository

```
git clone https://github.com/Aizhanaaah/sb-ecom.git
```

2. Open the project in IntelliJ IDEA.

3. Make sure dependencies are installed.

4. Run the Spring Boot application.

5. Test endpoints using:

* Postman
* Curl
* Browser

---

## Example JSON Response

```
[
  {
    "categoryId": 1,
    "categoryName": "Electronics"
  },
  {
    "categoryId": 2,
    "categoryName": "Books"
  }
]
```

---

