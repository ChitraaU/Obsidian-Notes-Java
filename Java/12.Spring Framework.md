***Strategy design pattern***
The Strategy Pattern defines a common interface for a family of algorithms, encapsulates each algorithm in a separate class, and allows the client to switch between them at runtime. It promotes composition over inheritance and follows the Open/Closed Principle because new strategies can be added without modifying existing code.

***Coupling***
The coupling basically refers to the degree of dependency of the classes with each .There can be tightly coupled classes and there can be loosely coupled classes

**Tight and Loose coupling**
*Tight Coupling :* When the two classes are highly dependent on each other which means that if there is a change in one class so that would be reflected in the other class also .

*Loose Coupling :* While in loose coupling the classes are not dependent on each other , it is achieved through interface and abstraction of the classes .Generally, we would make an interface and implement it to the class and then we would make it instance and make the object of the implemented class .Thus if any change has to be done , it would not directly impact any kind of major changes in the classes.

Interface
      ↑
Multiple Implementations
      ↑
Client depends on the Interface
      ↑
Choose the implementation at runtime

### Which is better tight coupling or loose coupling?

Loose coupling is better than tight coupling because it improves flexibility, reusability, and testability. In a loosely coupled design, changes or growth in the application affect only a few components, making the system easier to maintain and scale.![Coupling in Java](https://media.geeksforgeeks.org/wp-content/uploads/Untitled-28.png "Click to enlarge")

***Dependency Injection***
Dependency Injection is the process of providing an object with the dependencies it needs from outside, rather than having the object create those dependencies itself.
Dependency injection supports loose coupling.

- Constructor Injection
   The dependency is injected through a constructor 
- Setter Injection
   The dependency is injected through the setter.
 - Field Injection
   The dependency is injected through the field .


***Intro to web frameworks***

A framework is basically a collection of pre written codes ,libraries and rules that helps in building the application faster and with less effort

- what happens without a framework and with a framework
Without Spring framework, you would need to write code for:

- HTTP request handling
- Object creation
- Database connection
- Security
- Configuration
- Error handling
- Dependency management

That's thousands of lines of code.
With Spring Boot, much of this is already provided.
You mainly focus on your business logic.

# Framework vs Library

This is a very common interview question.
### Library

A library is a collection of reusable code.
You call the library whenever you need it.
Example:

```
Collections.sort(list);
```

Here **you** decide when to call the library.
**You control the flow.**

---

### Framework

A framework controls your application.
It tells you:

- where to write code
- how to organize it
- when your code will be executed
Example:

```
@RestController
public class StudentController {
}
```

You never call this controller yourself.
Instead, Spring calls it whenever an HTTP request arrives.
This is called **Inversion of Control (IoC)**.

***Spring as a framework***
***Concepts of Spring***

- its benefits
   - Promotes Loose coupling
   - Reduces the boilerplate code
   - Promotes Maintainability
   - Scalability

***Bean****
A bean is the Java object which the spring manages for the you(developer).

***Ioc Container**( Spring Container)*
 It is basically a container in the spring ,where it creates the beans ,inject the dependencies in them and manages the lifecycle of  beans.
 so its basically like a warehouse

***Application Context***
It is the main place of Spring Container implementation.
it stores the beans, manages them ,and resolve the dependencies.

***Inversion of Control***
When we create object using core java concepts then we have the control of when and how the objects are created while in spring that control is taken by the spring itself and it creates the objects for us . Thus ,it is called inversion of control

***The build tools***

> **A build tool is a tool that automates the process of building, managing, and organizing a software project, including managing its dependencies.**

For Java projects, the most common build tools you'll encounter are:

- **Maven**
- **Gradle**

### What does "building" actually mean?

Suppose you have:

src/

 ├── main/

 │    └── java/

 │         └── UserService.java

 └── test/

      └── UserServiceTest.java

Your build tool can automate things like:

Your source code

       ↓

Compile

       ↓

Run tests

       ↓

Package

       ↓

Create JAR
Instead of you manually doing all of that.
- Maven
- Gradle

### And dependency management

Suppose your application needs Jackson.

Without a build tool, you'd have to:

1. Find the correct JAR.
2. Download it.
3. Put it in your project.
4. Make sure its dependencies are also present.
5. Manage compatible versions.
build tools can also handle:

- Compilation
- Testing
- Packaging
- Dependency management
- Running plugins/tasks
- Creating JAR/WAR files
- Different build environments

pom file is  the file that handles the configurations and how the project should be built and what dependencies it should use

## Why is it called a "Project Object Model"?

Because Maven represents your project as a model containing information such as:

                pom.xml

                   │

       ┌───────────┼────────────┐

       ↓           ↓            ↓

    Project    Dependencies   Build

     info                      config

       │           │            │

       ↓           ↓            ↓

 groupId       Spring       Plugins

 artifactId    Hibernate    Compiler

 version       MySQL       Packaging

Maven reads this `pom.xml` and uses that information to perform the build.

### The easiest way to remember

> **`pom.xml` = the configuration/description file of a Maven project.**

And one very important thing: **POM is not Maven itself.** Maven is the **build tool**, while `pom.xml` is the **project configuration file that Maven reads**.

property tag is used for setter injection while constructor arg is used for constructor injection

***Inversion of Control***

This is concept which means that process of creating and managing the object goes to a framework and in this case it is Spring

***Dependency Injection***
When a class is dependent on the other class and when it is given to the class through a constructor, setter or a field it is called dependency injection.

What problems does Spring solve
 It injects the dependencies and manages the objects for the developer.
                    SPRING
                       │
                       ↓
                IoC Container
                       │
             Creates & manages
                       │
                       ↓
                    Beans
                       │
                       ↓
             Dependency Injection
                       │
             ┌─────────┼─────────┐
             ↓         ↓         ↓
        Constructor   Setter    Field
             │
             ↓
        Loose Coupling
             │
             ↓
      Flexible / Testable /
       Maintainable code