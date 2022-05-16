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

Then search for the missing dependencies: 

![search](https://user-images.githubusercontent.com/83961643/168551811-9ef92f8f-796a-49f7-b9be-04944f7df367.jpeg)

