# Spring MVC Architecture

Under the hood, Spring MVC applications are just Java Servlets. Software Engineers write their custom applications on top of (using) Spring MVC.

The benefits of having this architecture is that it sets a standard that other Developers can use and therefore provide better readability when many Developers are contributing to a code base.

# Request/ Response Lifecycle

An outline of the request/ response lifecycle can be found below. With an understanding of this, you can understand the workflow of Spring MVC. There are **three** main components of Spring MVC. The **Model**, the **View** and the **Controller** (MVC).

1. The User reaches an endpoint and an incoming request is passed to the Front Controller
2. The Front Controller delegates the request to another Controller
3. That other Controller handles the request and passes off to the backend components (perhaps a database)
4. The backend component hands a Model (data represented as a POJO) back to the other Controller
5. That other Controller delegates the rendering back to the Front Controller
6. The Front Controller passes the Model back to a View template
7. The View template renders the response.
8. Control is returned to the Front Controller which returns the resonse to the browser and thereby returning data to the User.

Again, each step is divided into three seperate parts:

1. Model - The Controller and Backend (data represented as a POJO)
2. View - The View templates and browser
3. Controller - Front controller and other Controllers