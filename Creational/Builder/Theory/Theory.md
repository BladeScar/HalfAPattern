**Intent:** Separate the construction of a complex object from its
representation so that the same construction process can create different
representations.

**Explanation:** When we talk about complex objects, we mean objects with multiple fields/member variables.
Such objects often require constructors with multiple(more then 3-4) parameters, while some of members might not need to be
initialised at creation, maybe not at all. Such situations force us to resort to multiple constructors which in turn
bloats the code(a.k.a [telescoping constructor anti-pattern](/../../blob/master/Glossary/TelescopingConstuctor.md)).

**Uses:** Use this pattern
* to allow step by step creation of an object(when not all of the components are needed for creation).
* to allow partial creation(to support different representations of the same general object).

**Comparisons to other patterns:** When it comes to creational patterns people think of the factory and abstract
factory patterns. The difference between them and the builder design pattern is that the intent of those two
is to facilitate polymorphism, while the builder is solving the telescoping anti-pattern and to separate the task
of creation of a complex object from that object.

**General UML Structure**
![alt text](Builder.png "Builder")

**Real world examples:**

* [java.lang.StringBuilder](http://docs.oracle.com/javase/8/docs/api/java/lang/StringBuilder.html)
* [Apache Camel builders](https://github.com/apache/camel/tree/0e195428ee04531be27a0b659005e3aa8d159d23/camel-core/src/main/java/org/apache/camel/builder)

**Credits**

* [Design Patterns: Elements of Reusable Object-Oriented Software](http://www.amazon.com/Design-Patterns-Elements-Reusable-Object-Oriented/dp/0201633612)