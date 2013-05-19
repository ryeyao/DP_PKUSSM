Design Patterns
====================
## Principles of Design ##

* SRP(Single Responsibility Principle)  

	+ A class should have one, and only one, reason to change  
	+ Every class should have a single responsibility, and that responsibility should be entirely encapsulated by the class.    
	+ ����һ������ԣ�Ӧ��ֻ��һ��������仯��ԭ��   

* OCP(Open-Close Principle)  

	* You should be able to extend a classes behavior, without modifying it.  
	* Software entities should be open for extension, but closed for modification.  
	* �����һ��ģ��ʱ��Ӧ��ʹ��ģ���ڲ����޸ĵ�ǰ���±���չ�������ڲ����޸�Դ���������¸ı��ģ�����Ϊ��  

* LSP(LisKov Substitution Principle)  

	* Derived classes must be substitutable for their base classes.  
	* In a computer program, if S is a subtype of T, then objects of type T may be replaced with objects of type S without altering any of the desirable properties of that program.    
 	* �������ࣨ���ࣩ�����ܹ��滻����ࣨ���ࣩ����ʹ�á���  
 	
* DIP(Dependency Inversion Principle)  

	Depend on abstactions, not on concretions.  
	
	* A. High-level modules should not depend on low-level modules. Both should depend on abstractions.  
	* ���߲�ε�ģ�鲻Ӧ�����ڵͲ�ε�ģ�飬���߶�Ӧ�������ڳ���ӿڡ�  
	* B. Abstractions should not depend upon details. Details should depend upon abstractions.  
	* ������ӿڲ�Ӧ�������ھ���ʵ�֣�����ʵ��Ӧ�ø������ڳ���ӿڡ�  
	
* ISP(Interface Segregation Principle)  

	* Make fine grained interfaces that are client specific.  
	* No client should be forced to depend on methods it does not use    
	* ��ʹ�ö��ר�ŵĽӿڱ��õ�һ�Ľӿ�Ҫ�á�  
	* ��һ���������һ�����������Ӧ�ý�������С�Ľӿ��ϡ�  
	
* CARP(Composite Resuse Principle or Composition Over Inheritance Principle)  

	* Classes may achieve polymorphic behavior and code reuse by containing other classes that implement the desired functionality instead of through inheritance.    
	* ��Ҫ����ʹ�úϳ�/�ۺϣ�������Ҫʹ�ü̳С�
	
* LoD(Law of Demeter or Principle of Least Knowledge)    

	* Each unit should have only limited knowledge about other units: only units "closely" related to the current unit  
	* Each unit should only talk to its friends; don't talk to strangers.  
	* Only talk to your immediate friends  
	
## GRASP (General Responsibility Assignment Software Patterns (ͨ��ְ��������ģʽ))
* Information Expert ��Ϣר��   
* Creator ������  
* Low Coupling �����  
* High Cohesion ���ھ�  
* Controller ������  
* Polymorphism ��̬  
* Pure Fabrication ���鹹  
* Indirection ���  
* Protected Variations �仯Ԥ��  

## GOF Design Patterns ##
### Creational
	Creational patterns are ones that create onjects for you, rather than having you instantiate objects directly. This gives your program more flexibility in deciding which objects need to be created for a given case

* ***Abstract Factory***  
	Groups object factories that have a common theme  
	
* Builder  
	Constructs complex objects by separating construction and representation
	  
* ***Factory Method***  
	Creates objects without specifying the exact class to create
	  
* Prototype  
	Creates objects by cloning an existing object
	  
* ***Singleton***  
	Restricts object creation for class to only one instance

### Structural
	These concern class and object composition. They use inheritance to compose interfaces and define ways to compose objects to obtain new functionality

* Adapter  
	Allows classes with incompatible interfaces to work together by wrapping its own interface around that of an already existing class
	
* ***Bridge***  
	Decouples an abstraction from its implementation so that the two can vary independently
	
* ***Composite***  
	Composes zero-or-more similar objects so that they can be manipulated as one object
	
* ***Decorator***  
	Dynamically adds/overrides behavior in an existing method of an object
	
* ***Facade***  
	Provides a simplified interface to a large body of code
	
* Flyweight  
	reduces the cost of creating and manipulating a large number of similar objects
	
* Proxy  
	provides a placeholder for another object to control access, reduce cost, and reduce complexity

### Behavioral
	Most of these design patterns are specifically concerned with communication between objects
	
* Chain of Responsibility  
	Delegates commands to a chain of processing objects
	
* ***Command***  
	Creates objects which encapsulate actions and parameters
	
* Interpreter  
	Implements a specialized language
	
* Iterator  
	Accesses the elements of an object sequentially without exposing its underlying representation

* Mediator  
	Allows loose coupling between classes by being the only class that has detailed knowledge of their methods

* Memento  
	Provides the ability to restore an object to its previous state (undo)

* ***Observer***  
	Is a publish/subscribe pattern which allows a number of observer objects to see an event

* ***State***  
	Allows an object to alter its behavior when its internal state changes

* ***Strategy***   
	Allows one of a family of algorithms to be selected on-the-fly at runtime

* ***Template method***  
	Defines the skeleton of an algorithm as an abstract class, allowing its subclasses to provide concrete behavior

* Visitor  
	Separates an algorithm from an object structure by moving the hierarchy of methods into one object
	 