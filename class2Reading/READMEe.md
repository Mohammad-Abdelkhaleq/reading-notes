# Code 401 - *Class 2 readings 

## Review: ES6 Classes

Classes are a template for creating __*objects*.
<hr>
Can a class declaration be hoisted? no 
<hr>

How would you describe a constructor and contextual “this” to a non-technical friend? 

*A constructor in JavaScript is a blueprint for creating objects. It defines how an object should be made and what properties and behaviors it should have.*

*The contextual "this" keyword in JavaScript refers to the current object being accessed or operated upon. It allows you to refer to the object's properties and methods without explicitly mentioning its name.*
<hr>

## Using Express Routing

Within Express, what does routing refer to?

*In Express, routing refers to the process of defining endpoints (URL paths) and handling requests to those endpoints. It involves mapping different URL patterns to specific functions or handlers that should be executed when a request is made to a particular endpoint. Routing helps in directing incoming requests to the appropriate code that should handle them, allowing you to define the logic and behavior of your web application.*
<hr>


What is the difference between a route path and a route method?

*Route Path: Defines the URL pattern or path that a request needs to match.*
*Route Method: Specifies the type of HTTP request that triggers a specific route handler.*

<hr>
When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?


*It is appropriate to add next as a parameter to a route handler or middleware in Express when you want to pass control to the next function in the middleware chain.*

*If next has been passed to your middleware as a parameter, you need to call next() within your middleware to pass control to the next middleware function. This allows the request to continue through the middleware chain and eventually reach the appropriate route handler or end the request-response cycle.*


<hr>

## Express Routing

What is an Express Router?

Express Router is a feature of Express that allows you to create modular and reusable sets of routes and middleware, enabling you to organize and manage routes more efficiently in your application. It helps in separating concerns and improving code organization.

<hr>

By what mean do we initialize express.Router() in an express server?

Create an instance of the Express Router using express.Router()

By initializing an Express Router and mounting it on a specific path in your Express application, you can separate and organize your routes and middleware into modular components


<hr>

What do we use route middleware for?


Route middleware in Express is used to perform additional operations on incoming requests or outgoing responses before or after the route handler is executed. It sits between the server receiving a request and the actual route handler function.