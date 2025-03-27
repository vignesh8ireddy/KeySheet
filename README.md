# Key Sheet

* src\main\java  
* src\main\resources
* src\main\target
* src\main\webapp
  * META-INF
  * WEB-INF

## =============JAVA STANDARD EDITION=============

## =============LOMBOK API=============

## =============JAVA ENTERPRISE EDITION=============

## =============SPRING FRAMEWORK=============
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

## =============SPRING BOOT=============
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

## =============SPRING DATA JPA=============

## =============SPRING TRANSACTION MANAGEMENT=============

## =============SPRING WEB / SPRING BOOT MVC=============

## =============REST API / RESTFUL WEBSERVICES=============

## =============SPRING CLOUD / MICROSERVICES=============

## =============SPRING SECURITY=============

## =============JMS JAVA MESSAGE SERVICE=============

## =============APACHE KAFKA=============

## =============SPRING MONGODB=============

## =============SPRING MAIL=============

## =============SPRING SCHEDULING=============

## =============SPRING BATCH=============

## =============SPRING AOP=============

## =============DESIGN PATTERNS=============

## =============SWAGGER API=============

## =============UNIT TESTING=============

## =============LOGGING=============

## =============DOCKER=============

## =============KUBERNETES=============

## =============JENKINS=============

## =============TERRAFORM=============

## =============ANSIBLE=============



### =============ZEPHYR=============

> A singleton class is made spring bean and configured multiple times with different bean id, what happens?
* Singleton pattern is broken and different object is created for each bean id.

> A singleton class is made spring bean with prototype scope, what happens when getBean(String,Class) method is called
multiple times over the class.
* Singleton pattern is broken, prototype scope is continued i.e multiple objects would be created for singleton class.

