**Intent:** Separate the construction of a complex object from its
representation so that the same construction process can create different
representations.

**Explanation:** When we talk about complex objects, we mean objects we multiple fields/member variables.
Such objects often require constructors with multiple parameters, while some of members might not need to be
initialised at creation, maybe not at all.

![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/Builder_UML_class_diagram.svg/500px-Builder_UML_class_diagram.svg.png "Builder")