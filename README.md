# Spring In Action 6th Edition
 Spring Frame Class Work by Craig Walls 

- [Download](https://spring.io)
- [Spring Initializr](https://start.spring.io)


> "Spring offers a container, reffered to as the Spring Application context. It creates and manages application components."
> 
> - Data persistance options
> - Microserve support
> - Reactive programming model
> - Runtime monitoring 
> - Security framework


[MVC](https://developer.mozilla.org/en-US/docs/Glossary/MVC)
(Model-View-Controller) is a pattern in software design commonly used to implement user interfaces, data, and controlling logic. It emphasizes a separation between the software's business logic and display. This "separation of concerns" provides for a better division of labor and improved maintenance. Some other design patterns are based on MVC, such as MVVM (Model-View-Viewmodel), MVP (Model-View-Presenter), and MVW (Model-View-Whatever).

1. Model: Manages data and business logic.
2. View: Handles layout and display.
3. Controller: Routes commands to the model and view parts.

![Data-3](https://user-images.githubusercontent.com/83961643/168585490-596f7939-338f-465b-a788-c44d0c16aa7d.png)



[Annotation note reference](https://springframework.guru/spring-framework-annotations/)

@Configuration 

This annotation is used on classes which define beans. `@Configuration` is an analog for XML configuration file – it is configuration using Java class. Java class annotated with `@Configuration` is a configuration by itself and will have methods to instantiate and configure the dependencies.

@Bean 

This annotation is used at the method level. `@Bean` annotation works with `@Configuration` to create Spring beans. As mentioned earlier, `@Configuration` will have methods to instantiate and configure dependencies. Such methods will be annotated with `@Bean`. The method annotated with this annotation works as bean ID and it creates and returns the actual bean.


Spring Initializer:
![init](https://user-images.githubusercontent.com/83961643/168547650-8081738f-3227-4faa-b559-9096aeb5ec10.jpeg)

How to make a New Project: 

![grsb](https://user-images.githubusercontent.com/83961643/168549660-d9669ab9-5245-4eb5-88e2-035b52e9a935.jpg)


Create New Project: 

![new](https://user-images.githubusercontent.com/83961643/168550324-01aa74f7-3ed3-4c68-a365-e93e2cd002c9.jpeg)

Click Next and wizard takes you to setting up dependencies: 
![dev](https://user-images.githubusercontent.com/83961643/168551501-b9f187cc-1c50-4aa4-a9d5-84f196b761fe.jpeg)

Then search for the missing dependencies eg. Spring Web and add it: 

![search](https://user-images.githubusercontent.com/83961643/168551811-9ef92f8f-796a-49f7-b9be-04944f7df367.jpeg)

How the project looks once you click Finish and it has finished loading: 

![project](https://user-images.githubusercontent.com/83961643/168552351-8bd9a05d-7682-4908-887c-b0419992d1ad.jpeg)

More about the files: 

![files](https://user-images.githubusercontent.com/83961643/168552485-d0c2d252-a011-44ce-bfcc-652be3a553d7.jpeg)

Open the Taco Test File to view this code: 

![taco](https://user-images.githubusercontent.com/83961643/168555611-c773fe43-6b69-4f13-bc08-610bf5fda0c0.jpeg)

Running the Maven Test File:

![runtest](https://user-images.githubusercontent.com/83961643/168558725-05798f8e-64b1-4314-960b-f5b484655f88.jpeg)

![run](https://user-images.githubusercontent.com/83961643/168558378-3bb110c4-f9ff-4ed6-a6c9-d685e0aaf698.jpeg)


Create a new class in the tacos package: 

![createclass](https://user-images.githubusercontent.com/83961643/168559951-557d582f-b9a2-482c-a787-74fb0ad44130.jpeg)


Adding the code to the home controller class:

![homecontroller](https://user-images.githubusercontent.com/83961643/168560739-d2ffd9c4-1757-4666-b93d-b807b1fc64e7.jpeg)


[Annotation note reference](https://springframework.guru/spring-framework-annotations/)
 
@Component

This annotation is used on classes to indicate a Spring component. The `@Component` annotation marks the Java class as a bean or say component so that the component-scanning mechanism of Spring can add into the application context.

@Service 

This annotation is used on a class. The `@Service` marks a Java class that performs some service, such as execute business logic, perform calculations and call external APIs. This annotation is a specialized form of the `@Component` annotation intended to be used in the service layer.

@Repository 

This annotation is used on Java classes which directly access the database. The `@Repository` annotation works as marker for any class that fulfills the role of repository or Data Access Object.

This annotation has a automatic translation feature. For example, when an exception occurs in the `@Repository` there is a handler for that exception and there is no need to add a try catch block.

@GetMapping

This annotation is used for mapping HTTP GET requests onto specific handler methods. `@GetMapping` is a composed annotation that acts as a shortcut for `@RequestMapping`(method = RequestMethod.GET)


Create a new HTML file in the template folder under src:
![html](https://user-images.githubusercontent.com/83961643/168561961-12d99d4d-007d-4d67-9657-5263fd53624d.jpeg)



Add your taco image and images folder to the static folder:

![images](https://user-images.githubusercontent.com/83961643/168562438-97bfe10b-2e2c-4538-af77-a6c149512b22.jpeg)


Create a Test File:

![test class](https://user-images.githubusercontent.com/83961643/168563958-b700961e-61c1-435c-81be-88e014e80f63.jpeg)

Run the test in IDE: 
`$ mvnw test`


Run Spring Boot App:

![runspringbootapp](https://user-images.githubusercontent.com/83961643/168565373-1f163d9d-30b5-4734-a32a-270a3da99d5c.jpeg)

Open your borswer and search localhost:8080

![localhost8080](https://user-images.githubusercontent.com/83961643/168565703-334f47fb-ff14-4a83-9e03-8cb49ec3053d.jpeg)


[How do I install and use the browser extensions?](http://livereload.com/extensions/)
Download & open to install:

- [Safari extension 2.1.0](http://download.livereload.com/2.1.0/LiveReload-2.1.0.safariextz) — note: due to Safari API limitations, browser extension does not work with file: URLs; if you’re working with local files via file: URL, please use Chrome or insert the SCRIPT snippet.

- [Chrome extension on the Chrome Web Store](https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei) — if you want to use it with local files, be sure to enable “Allow access to file URLs” checkbox in Tools > Extensions > LiveReload after installation.

- [Firefox extension 2.1.0](https://addons.mozilla.org/en-US/firefox/addon/livereload/) from addons.mozilla.org.

> Insight into the data your application is working with: 
> http://localhost:8080/h2-console 


### Spring Dependencies:

## The Core Spring Framework

## Spring Boot

## Spring Data

## [Spring Security](https://www.baeldung.com/spring-security-with-maven)
 ### spring-security-core
 `<properties>
    <spring-security.version>5.3.4.RELEASE</spring-security.version>
    <spring.version>5.2.8.RELEASE</spring.version>
</properties>
<dependency>
    <groupId>org.springframework.security</groupId>
    <artifactId>spring-security-core</artifactId>
    <version>${spring-security.version}</version>
</dependency>`
 
 ### spring-security-web
 `<dependency>
    <groupId>org.springframework.security</groupId>
    <artifactId>spring-security-web</artifactId>
    <version>${spring-security.version}</version>
</dependency>`

 ### spring-security-config 
`<dependency>
    <groupId>org.springframework.security</groupId>
    <artifactId>spring-security-config</artifactId>
    <version>${spring-security.version}</version>
</dependency>`

## Spring Integration and Spring Batch

## Spring CLoud 

## Spring Native 

Instead of starting from scratch, import chapter 1 code as a starter for chapter 2:

![imports](https://user-images.githubusercontent.com/83961643/168578745-f3a7d31b-2d77-459e-acd1-f0b2e0f5181e.jpeg)

Please note that doing it this way will sow down your machince and will take a while to load. Rather start a new file or build on the pervious version. 


## Lombok

[Lombok tutorial](https://projectlombok.org/#)

Add -> Spring -> Add Starters -> SELECT POM file 

![springlombokstarter](https://user-images.githubusercontent.com/83961643/168580226-f08abe24-c384-4dc0-9491-9ba3adda44ea.jpeg)
![clickpom](https://user-images.githubusercontent.com/83961643/168580235-f5d1550c-0662-407b-a3f6-0607382964c0.jpeg)


Watch this [tuotorial](https://www.youtube.com/watch?v=Xx3urDhrN_M) if you aren't sure how to save your jar file that you have downloaded from the [Project Lombok](https://projectlombok.org/download) web page. 

![jar](https://user-images.githubusercontent.com/83961643/168582462-f7ec2ca4-ac8d-4ae8-99e6-9c691f1e1f7c.jpeg)
![install](https://user-images.githubusercontent.com/83961643/168582477-9682c8d6-65b2-4421-9e12-6f603baa227a.jpeg)
![java](https://user-images.githubusercontent.com/83961643/168582480-031aa57e-ca49-4962-8a34-487aa40dce52.jpeg)
![waiting](https://user-images.githubusercontent.com/83961643/168582482-7d31ae29-07b4-450c-be5f-83332f3c3c5b.jpeg)


## Simple Logging Facade for Java [SLF4J](https://www.slf4j.org)

Serves as a simple facade or abstraction for various logging frameworks (e.g. java.util.logging, logback, log4j) allowing the end user to plug in the desired logging framework at deployment time.
[READ THE MANUAL](https://www.slf4j.org/manual.html)

![concrete-bindings](https://user-images.githubusercontent.com/83961643/168597598-696d8c16-260c-4dd3-bcda-a248614d4a97.png)

![summary](https://user-images.githubusercontent.com/83961643/168597627-2da192df-1b17-49e5-bb91-6b7363f0317e.jpeg)


## Designing the view

- JavaServer Pages (JSP)
- Thymeleaf 

`<p th:text="${message}">placeholder message</p>`:Thymeleaf templates are just HTML with some additional element attributes that guide a template in rendering request data. 

`${}`: operator tells it to use the value of a request attribute ("message", in this case).

`th:each`:iterates over a collection of elements, rendering the HTML once for each item in the collection.

- FreeMarker
- Mustache
- Groovy-based templates


## `localhost:8080/design` in your browser to view 
![design](https://user-images.githubusercontent.com/83961643/168756686-bf315392-88e4-4fa3-98f9-c5150cb7abf6.jpeg)

The Taco OrderForm.html File 

![page2](https://user-images.githubusercontent.com/83961643/168758140-5cf71a20-6c4f-4239-ade2-b105ad051c6f.jpeg)


Spring supports the JavaBean Validation API [JSR 303](https://jcp.org/en/jsr/detail?id=303) 
![java](https://user-images.githubusercontent.com/83961643/168760101-a2dfb833-ae8b-479d-bc91-55a3bd46e8bd.jpeg)


## Adding a Valedation dependency to your pom.xml file:
Right click on your pom file and say Spring -> Add Starters 
Then you will see this pop up 
![validation](https://user-images.githubusercontent.com/83961643/168761553-405902f7-898e-4efd-8fec-1b263909c59c.jpeg)
![step](https://user-images.githubusercontent.com/83961643/168761595-5caaa82d-d0af-4fb8-8910-4f072b0f0d9a.jpeg)

Select pom only:

![pom](https://user-images.githubusercontent.com/83961643/168761642-1368b634-d34b-4b91-b2c8-4fd89ab737f2.jpeg)

This is the new code you will have in your file:

![added](https://user-images.githubusercontent.com/83961643/168761663-446cfab1-ed46-45b4-b7fb-fa2013fa99ea.jpeg)


## The Luhn Algorithm for Credit Card Validation
`@CreditCardNumber` 
`ccNumber` property
[Luhn algorithm check](https://www.creditcardvalidator.org/articles/luhn-algorithm)

#### How to calculate a Luhn checksum:
> 1. From the rightmost digit (the check digit), move left and double the value of every second digit; if doubled number is greater than 9 (e.g., 7 × > 2 = 14), then subtract 9 from the product (e.g., 14: 14 - 9 = 5). 
> 2. Sum of all the digits in the newly calculated number.
> 3. Multiply the sum by 9, the Luhn check digit is the rightmost digit of the result (e.g, the result modulo 10).

In the following example, we use a sample credit card number "7992739871", with an unknown Luhn check digit at the end, displayed as 7992739871x:
![luhn](https://user-images.githubusercontent.com/83961643/168764562-178d6ace-e6fd-4cf7-a15b-98f2bf1ee360.jpeg)

The sum of all the digits in the third row above is 67+x.

We still need to calculate the check digit, X. The check digit can be obtained by computing the sum of the non-check digits then computing 9 times that value modulo 10. For our example, the equation is 67 × 9 mod 10. Broken down in more detail:

1. Compute the sum of the non-check digits (67).
2. Multiply by 9 (603). 
3. The units digit (3) is the check digit. Thus, x=3.

## Domain Driven Design (DDD) 
Core concepts of DDD: Aggregates and aggregate roots - a design approach that promotes the idea that the structure and language of software code should match the business domain.

![Data-3](https://user-images.githubusercontent.com/83961643/168805609-b8afe6f2-05d9-4ea7-8e40-ed6111a4d3b0.png)

Read for more info on the topic [Domain-Driven Design: Tackling Complexity in the Heart of Software](https://www.dddcommunity.org/book/evans_2003/)


## Selenium jar 
Download your selenium jar file then follow these steps..

in your menu select build path

![seleniumbuildpath](https://user-images.githubusercontent.com/83961643/169252606-fc302e56-b3ad-4188-8fc7-48d443f22c82.jpeg)

Go into your library and choose add extrnal jar and select your jar file.

![library_addExternalJar](https://user-images.githubusercontent.com/83961643/169252631-fb6e054f-414d-4f29-a78d-4b35c647393d.jpeg)

![chooseyourseleniumjar](https://user-images.githubusercontent.com/83961643/169252633-818f940e-43c7-4d4e-a93b-608048db289a.jpeg)

Watch this video if you are struggling with your selenium dependency: [Tutorial](https://www.youtube.com/watch?v=beWEdwfjF28)

What the new login form looks like after Chapter 5
![workinglogin](https://user-images.githubusercontent.com/83961643/169278662-ddbe9f4d-3fc2-4585-977a-8c9e702c30ab.jpeg)


## Configuration

> *Fine-tuning configuration*
> - Bean wiring: Configuration that declares application components to be created
as beans in the Spring application context and how they should be injected into
each other
> - Property injection: Configuration that sets values on beans in the Spring application
context
![Data-4](https://user-images.githubusercontent.com/83961643/169283300-3751813c-9489-451b-b8f5-192117c78106.png)


## YAML 

_Known as ain’t markup language OR yet another markup language_
[More Info Here](https://www.redhat.com/en/topics/automation/what-is-yaml)

> - Features that come from Perl, C, XML, HTML, and other programming languages. YAML is also a superset of JSON, so JSON files are valid in YAML.
> - Python-style indentation to indicate nesting. 
> - Tab characters are not allowed, so whitespaces are used instead. There are no usual format symbols, such as braces, square brackets, closing tags, or quotation marks. 
> - YAML files use a .yml or .yaml extension. 
> - The structure of a YAML file is a map or a list.
> - Contains scalars, which are arbitrary data (encoded in Unicode) that can be used as values such as strings, integers, dates, numbers, or booleans.

More YAML examples and usage:
[1](https://stackabuse.com/reading-and-writing-yaml-files-in-java-with-jackson/)
[2](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started)
[3](https://phoenixnap.com/blog/what-is-yaml-with-examples)


## REST services
HTTPie is making APIs simple and intuitive for those building the tools of our time.
[httpie](https://httpie.io/)


Testing the api 
![api](https://user-images.githubusercontent.com/83961643/169297586-825ed5bd-08aa-4c8d-bc02-a972f28a2824.jpeg)

CommandLine test in Terminal 

![commandlinetest](https://user-images.githubusercontent.com/83961643/169298049-280470c7-ff6f-4389-8cf9-9a4957d9fa2f.jpeg)

RESTful Controllers:
![restful](https://user-images.githubusercontent.com/83961643/169476051-6f5742b0-246b-4fd5-b1e6-816d4a23c51f.jpeg)


