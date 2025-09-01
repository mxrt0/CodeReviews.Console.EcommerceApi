# E-Commerce API
E-Commerce API for selling PC components. Developed with C# and SQLite.

## Given Requirements
* The project needs to be an ASP.NET Core Web API, with Entity Framework and SQL Server / SQLite
* The API needs to use Dependency Injection
* There should be at least 3 tables: Products, Categories and Sales
* Products and Sales need to have a many-to-many relationship, meaning products can have multiple sales, and sales can have multiple products
* Products need to have a price. Multiple products can be sold in the same sale
* There needs to be provided a JSON Postman Collection with all possible requests for the API in the PR
* There is no need to create an UI to consume the API
* The GetProducts and GetSales endpoints need to have pagination capabilities
* In retail it's good practice to prevent deletion of records. Soft-deletes are permitted.
* Products prices shouldn't be updated. 

## Features
* Simple API where users can send different requests (provided in the Postman collection)
* Ability to make sales, add products and categories
* Solely EF-managed SQLite database workflow

## Challenges

* Creating Pagination capabilities
* Organizing the Postman collection (first-time)
* Managing to return appropriate status codes on responses

## Lessons Learned
* Pagination is important
* It is important to return sensible request status codes
* Important to handle server-side and client-side errors properly

## Areas To Improve
* Request Status Codes
* Postman 

## Resources
* Postman Client for testing API

## Configuration Instructions
* Located in the project folder of the API is an app.Development.json.example file that contains the structure of the configuration. User should configure DB path as desired.
* After that, copy the contents of the file onto an actual app.Development.json that is also placed within the API project folder.


