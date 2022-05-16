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


