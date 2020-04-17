# Vocabulary

The following is a list of important terms that we will use to describe different components of Spring MVC. Familiarize yourself with them.

### DispatcherServlet

The entry/ configuration point for the application. The Front Controller.

### Controller

A command pattern object that handles the request and determines which View to route to.

### RequestMapping

The URL and request type that a Java method is tied to. This handles HTML requests like GET, PUT, etc.

### ViewResolver

This is used to locate JSP pages or whatever view we are using.

### Servlet-config

Configuration file per DispatcherServlet. This is how Spring knows how to configure things and "wire up" our application.

### POJO

Plain Old Java Object. Generally has a no arguments constructor and private member variables exposed through getters and setters.

### Bean

A Spring configured POJO. It is an object that has been instantiated with Spring and is "wired up" to be used inside our custom Spring application.