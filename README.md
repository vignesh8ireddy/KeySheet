# Key Sheet


## =============| JAVA STANDARD EDITION |=============

* 
* Java Bean (5 Standards, 3 Classic examples: VO, DTO, BO)

* Concrete class, Abstract class, Interface | Concrete method, Abstract method, Null method
* java.time API introduced in java 8 addresses the shortcomings of the older java.util.Date and java.util.Calendar 
classes.
* 

## =============| LOMBOK API |=============
* @Setter, @Getter, @AllArgsConstructor, @NoArgsConstructor, @RequiredArgsConstructor and @NonNull, @ToString, @EqualsAndHashCode
* @Data (@Setter, @Getter, @RequiredArgsConstructor, @ToString, @EqualsAndHashCode)
* @Retention(SOURCE) of every lombok annotation
* Object.toString() X @ToString of lombok
* Object.equals(), Object.hashCode() X @EqualsAndHashCode of lombok
* @Data will generate RequiredArgsConstructor only when @AllArgsConstructor and/or @NoArgsConstructor are not placed.
If @AllArgsConstructor and/or @NoArgsConstructor are/is placed, then use @RequiredArgsConstructor along with @Data.

## =============| JAVA ENTERPRISE EDITION |=============
* Programming Language X Language Technology X Framework
* Application Server X Web Server X Database Server
* Catalina Container, 5 operations on a servlet component
  * Load component class, Create instance, Manage instance, Call life cycle methods, Destroy instance.
* Web Server Responsibilities
  * Builtin JRE
  * Provides Web Container (has both Catalina container and Jasper container)
  * Security, Logging, Auditing,..
  * Requests and Responses
* Daemon Process (best example: Windows Task Manager)
* Upto version 6 Tomcat is a Webserver and from version 7, Tomcat is an application server.
* Servlets using Servlet API and JSP API

* 3 ways of Configuring servlet component with catalina container.
* Project Directory Structures
  * Project in src folder
    * src\project
  * Project in src\main\java folder
    * src\main\java\
    * src\main\resources
    * src\main\target
    * src\main\webapp
      * META-INF
      * WEB-INF
    * src\test\java
    * src\test\resources
## =============| SPRING FRAMEWORK |=============
* Maven + 7 Spring jar files (spring-context-support, spring-context, spring-core, spring-beans, spring-aop, spring-jcl,
spring-expression)
* Java Bean/Component
* Container: Catalina, Jasper, IOC
  * BeanFactory Container Vs ApplicationContext Container
  * Life Cycle of a spring bean
  * Dependency Lookup
  * Dependency Injection (or) Bean Wiring
    * XML Approach, XML + Annotations Approach, only Annotations Approach
  * getBean(String,Class)
  * getEnvironment()
  * AnnotationConfigApplicationContext.class
* @Configuration (Stereotypes)
* @ComponentScan(basePackages)
* @Bean(name)
* @Component
* @Autowired
* NoUniqueBeanDefinitionException, @Qualifier, @Primary or matching bean_id
* Field Injection X Constructor Injection X Method Injection X Arbitrary Method Injection
* Spring Bean Scope, @Scope : singleton (bydefault) X prototype X request X session X application X websocket
* Eager-Instantiation X Lazy-Instantiation, @Lazy(boolean) for singleton scope beans.
* Other stereotypes: @Controller, @Service, @Repository
* @PropertySource(value=String), @Value("$xxxx")
* Environment.class and getProperty(), how to inject this spring bean? - @Autowired X getEnvironment()
* @ImportResource(String), src\main\resources\applicationContext.xml
* A spring bean life cycle: Bean Loading, Instantiation, Dependency Injection, @PostConstruct, Business methods, 
@PreDestroy, DeInstantiation, Bean Unloading

## =============| SPRING BOOT |=============
* Spring boot starter jar files makes Spring Boot powerful than Spring Framework
* Spring Boot X Spring Framework
  * Autoconfiguration of certain spring beans
  * Auto dependency injection of certain spring beans
  * Auto provision of dependant and relevant jar files
  * Embedded database servers
  * Provision database connectivity configurations
  * Embedded application servers
  * Plugin for maven and gradle tools
* @SpringBootApplication, @EnableAutoConfiguration, SpringApplication.run(Class, String[])
* Three thumb rules while working with Spring Boot.
* Other stereotypes: @RestController, @ControllerAdvice

## =============| SPRING DATA JPA |=============

## =============| SPRING MONGODB |=============

## ======| SPRING TRANSACTION MANAGEMENT |======

## =============| SPRING WEB / SPRING BOOT MVC |=============
* MVC X Monolithic
* MVC Application Components: FrontController, Controller classes, HandlerMapping, View components and View Resolver
* DispatcherServlet: FrontController servlet given by spring-web starter.
* Spring MVC X Spring Boot MVC
* Background operations when a spring boot mvc application is deployed over an application server.
* Maven Dependencies: spring-web, spring dev-tools API, Apache JSTL-API
* application.properties:
  * spring.mvc.view.prefix
  * spring.mvc.view.suffix
  * server.port
  * server.servlet.context-path
* webapps/WEB-INF/
  * classes
  * lib
  * config
  * pages
* @RequestMapping(String), @GetMapping(String), @PostMapping(String),...
* Request Paths: start with "/", default one, multiple request paths,
* Spring Boot MVC Application Working
* Embedded Tomcat Server provided by Spring Boot, tomcat-embed-jasper maven dependency.
* Data Rendering and Shared Memory
  * Map (I)
  * Model (I)
  * BindingAwareModelMap (C)
  * HashMap (C)
* Cases where request path of a handler method becoming logical view name for the request
* ModelAndView(C), legacy style of data rendering and returning logical view name.
* Handler method chaining: forward X redirect
* Using PrintWriter(C) instead of View components
* Rendering Collections, Arrays, Model(C) instance, array of Model(c) instances,...
* One-Way Data Binding:
  * HTML form elements' name attribute
  * Candidate(C)
  * 
* Two-Way Data Binding:

## =============| REST API / RESTFUL WEBSERVICES |=============

## =============| SWAGGER API |=============

## =============| SPRING CLOUD / MICROSERVICES |=============

## =============| DESIGN PATTERNS |=============
* 23 GoF Patterns
  * Creational Patterns
    * Singleton, Factory, Abstract Factory, Builder, Prototype
  * Structural Patterns
    * Adapter, Decorator, Flyweight, Proxy, Facade, Composite, Bridge,...
  * Behavioral Patterns
    * Chain of Responsibility, Template, Strategy, Command, Interpreter, Iterator, Mediator, Momento, Observer, State,
    Visitor,...
* JEE Patterns [client Tier, Presentation Tier, Business Tier, Integration Tier, Resource Tier]
  * Presentation Tier
    * Front Controller, Intercepting Filter, Application Controller, Context Object, View Helper, Composite View,
    Service to Worker and Dispatcher View
  * Business Tier
    * Business Delegate, Service Locator, Service Facade, Application Service, Business Object, Composite Entity,
    Transfer Object, Transfer Object Assembler, Value List Handler,...
  * Integration Tier Patterns
* Microservices Patterns


## =============| SPRING SECURITY |=============

## =============| SPRING MAIL |=============

## =============| SPRING SCHEDULING |=============

## =============| SPRING BATCH |=============

## =============| SPRING JDBC |=============

## =============| JMS JAVA MESSAGE SERVICE |=============

## =============| APACHE KAFKA |=============

## =============| SPRING AOP |=============

## =============| GRAPHQL |=============

## =============| UNIT TESTING |=============

## =============| LOGGING |=============

## =============| DOCKER |=============

## =============| KUBERNETES |=============

## =============| JENKINS |=============

## =============| TERRAFORM |=============

## =============| ANSIBLE |=============

## =============| SPRING AI |=============


## =============| ZEPHYR |=============

> A singleton class is made spring bean and configured multiple times with different bean id, what happens?
* Singleton pattern is broken and different object is created for each bean id.

> A singleton class is made spring bean with prototype scope, what happens when getBean(String,Class) method is called
multiple times over the class.
* Singleton pattern is broken, prototype scope is continued i.e multiple objects would be created for singleton class.

> Is Constructor overloading and overriding possible?
* Constructor overloading is possible and very common, but constructor overriding is not possible because subclass'
constructor name is not same as superclass'.

> What happens when there is an infinite loop in the constructor chaining, CTE or RTE?
* CTE: Compile-Time Error

> Is it possible to generate a constructor with var-args using lombok api?
* No

> What kind of request does a hyperlink generates?
* GET request
