**Intent:** Separate the construction of a complex object from its
representation so that the same construction process can create different
representations.

**Explanation:** When we talk about complex objects, we mean objects with multiple fields/member variables.
Such objects often require constructors with multiple parameters, while some of members might not need to be
initialised at creation, maybe not at all.

**Uses:** In general we use this pattern when we want to avoid cluttering the an object with to many 
constructors.

**General UML Structure**
![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/Builder_UML_class_diagram.svg/500px-Builder_UML_class_diagram.svg.png "Builder")

**Real world examples:**

* [java.lang.StringBuilder](http://docs.oracle.com/javase/8/docs/api/java/lang/StringBuilder.html)
* [Apache Camel builders](https://github.com/apache/camel/tree/0e195428ee04531be27a0b659005e3aa8d159d23/camel-core/src/main/java/org/apache/camel/builder)

**Credits**

* [Design Patterns: Elements of Reusable Object-Oriented Software](http://www.amazon.com/Design-Patterns-Elements-Reusable-Object-Oriented/dp/0201633612)