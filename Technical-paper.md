# Spring MVC (Model View Controller)
## MVC Architecure
The MVC architecture was developed to make development of web applications in rapid and parallel manner. If an MVC model is used to develop any particular web application then it is possible that the application can be developed three times faster than normal development. This is possible because the Model, View and Controller can be developed by three developers parallely at the same time. 

### Model 
   
Model contains the data of the application. Data can be single object or collection of objects.

### View

View represents the provided information in a particular format. Generally, JSP+JSTL is used to create a view page.

### Controller

Controller contains the business logic of an application. Here, the @Controller annotation is used to mark the class as the controller.

![mvc](https://github.com/user-attachments/assets/1d1db8d6-0ad9-43b4-9cba-900ab05ce4fa)


## Spring MVC

A Spring MVC is a Java framework which is used to build web applications. It also follows the Model-View-Controller design pattern. It implements all the basic features of a core spring framework like Inversion of Control, Dependency Injection. A Spring MVC provides an elegant solution to use MVC in spring framework by the help of DispatcherServlet. Here, DispatcherServlet is a class that receives the incoming request and maps it to the right resource such as controllers, models, and views.

Spring Model-View-Controller Flow Diagram

![Spring-MVC-Framework-Control-flow-Diagram](https://github.com/user-attachments/assets/fde11e38-f303-47fe-9af5-612183716236)

Spring MVC Framework works as follows

* All the incoming requests are intercepted by the DispatcherServlet that works as the front controller.
* The DispatcherServlet then gets an entry of handler mapping from the XML file and forwards the request to the controller.
* The object of ModelAndView is returned by the controller.
* The DispatcherServlet checks the entry of the view resolver in the XML file and invokes the appropriate view component.

    
The following example shows DispatcherServlet declaration and mapping:

<web-app>

    <servlet>
        <servlet-name>example</servlet-name>
        <servlet-class>org.springframework.web.servlet.DispatcherServlet</servlet-class>
        <load-on-startup>1</load-on-startup>
    </servlet>

    <servlet-mapping>
        <servlet-name>example</servlet-name>
        <url-pattern>/example/*</url-pattern>
    </servlet-mapping>

</web-app>

## Use Cases of Spring MVC

* ### Web Application Development
   Spring MVC is primarily designed for building web applications. It provides a structured and modular approach to develop scalable and maintainable web-based systems.
 * ### Enterprise-Level Applications
   Spring MVC is well-suited for developing enterprise-level applications where the separation of concerns and scalability are crucial. It integrates seamlessly with other components of the Spring Framework, such as Spring Security and Spring Data.
* ### RESTful Web Services
   Spring MVC is used to build RESTful web services by leveraging the features of the framework, including the ability to produce and consume JSON or XML payloads. It is commonly chosen for implementing the backend of RESTful APIs.
* ### Interactive Websites
   Spring MVC is employed for creating interactive and dynamic websites that require server-side processing and interaction. It is often used in conjunction with frontend frameworks like Angular, React, or Vue.js to build modern, single-page applications.
* ### Content Management Systems (CMS)
   Spring MVC is suitable for building content management systems where content creation, modification, and presentation need to be managed through a web interface. The modular structure of Spring MVC facilitates the development of extensible CMS applications.


## Advantages of Spring MVC Framework 


### 1.Predefined Templates
 
 Spring framework provides templates for JDBC, Hibernate, JPA etc. technologies. So there is no need to write too much code. It hides the basic steps of these         technologies.

### 2.Loose Coupling 

The Spring applications are loosely coupled because of dependency injection.

### 3.Easy to test 

The Dependency Injection makes easier to test the application. The EJB or Struts application require server to run the application but Spring framework doesn’t require server.
   
### 4.Lightweight 

Spring framework is lightweight because of its POJO implementation. The Spring Framework doesn’t force the programmer to inherit any class or implement any interface.
   
### 5.Fast Development 

The Dependency Injection feature of Spring Framework and it support to various frameworks makes the easy development of JavaEE application.
   
### 6.Powerful abstraction 

It provides powerful abstraction to JavaEE specifications such as JMS, JDBC, JPA and JTA.

## References

* https://docs.spring.io/spring-framework/docs/3.2.x/spring-framework-reference/html/mvc.html
* https://www.geeksforgeeks.org/spring-mvc-framework/
* https://frontend.turing.edu/lessons/module-3/mvc.html

