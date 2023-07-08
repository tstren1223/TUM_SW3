Facade Pattern
The Facade Pattern reduces the coupling of subsystems by encapsulating the functionality of a complex subsystem. A Facade hides implementation details and only exposes the desired functionality in an easily accessible way to the client.

Problem Statement
The COVID-19 pandemic forces local stores to digitalize their business. The new startup ECommerce provides the infrastructure for handling the ordering and shipping process. For one of its first clients, the Cinema, the startup also takes care of playing and creating advertisements. Your friend Bob works at ECommerce, and when you heard they were looking for developers, you immediately joined them as a working student.

Your Task
Currently, stores can access functionalities they should not be able to access. Furthermore, some clients are overwhelmed with the controller system. Your first task at ECommerce is to resolve this issue by refactoring Bob's code and introducing the facade pattern. Implement the facade according to the UML diagram below that Bob has prepared for you.

You have the following tasks:

1. Introduce the Facade
 Add ECommerceFacade 2 of 2 tests passing
Add a new class called ECommerceFacade to your project. In this class, you will in the following implement the methods of the facade.

2. Implement the Facade
 Add public methods to the facade 3 of 3 tests passing
Implement all the public methods from the classes OrderController and AdvertisementController in the facade by delegating their functionality to the respective controller methods. Make sure that each controller is initialized in the constructor.
 Implement the shipOrder method 3 of 3 tests passing
Implement a new shipOrder method which receives an order and an address as parameters. Use the createShipping method of the ShippingController to create the shipping for the passed arguments. Make sure to set the shipping of the passed order before calling shipOrder on the ShippingController.
3. Reduce the coupling
 Remove associations to the controller classes and add associations to the facade 4 of 4 tests passing
Remove the associations between Cinema and the three controllers: OrderController, ShippingController and AdvertisementController. The same applies to OrderController, ShippingController and BookStore.
Add associations to the ECommerceFacade in the classes of the package store and implement the functionality in these classes by invoking methods on the ECommerceFacade.

UML Diagram# TUM_SW3
<img width="757" alt="image" src="https://github.com/tstren1223/TUM_SW3/assets/64294878/9edb88c8-e6ca-4549-8201-b2cd8122b660">
