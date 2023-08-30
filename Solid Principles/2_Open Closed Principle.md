- The Open Close Principle states that the design and writing of the code should be done in a way that new functionality should be **added with 
minimum changes** in the existing code. The design should be done in a way to allows the adding of new functionality as new classes, keeping 
as much as possible existing code unchanged.

- **Ex:** Imagine that the system uses classes that implement **TaxCalculator interface** in order to calculate taxes.
In such a system, replacing IndiaTaxCalculator with NepalTaxCalculator (assuming, of course, that both of them implement TaxCalculator)
will allow quickly adapt the system’s tax calculation policy from Indian market to the Nepal market.

- Above Process does not require modification of the existing logic – all we need to do is provide a new implementation of
an existing interface.

## Methods to achieve OCP
- Using Extension methods
- Using Classes, Abstract class, or Interface-based Inheritance
- Generics
- Composition 
