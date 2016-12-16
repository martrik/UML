# Class Diagram

## Constructors, Getters, and Setters
For the sake of brevity and in order to keep the UML as compact as possible we decided to only mention Constructors that are not default constructors in the class diagram. Furthermore, we made most of our variables private, but didn't specify Getters and Setters in the Class Diagram, as this would increase the number of methods in and the overall size of the class diagram unnecessarily.

## Classes and structs without connections
Some of our classes and structs are not connected to any other class. The reason for that is that they are never "associated" or kept as a state anywhere in the program, but are just temporary intermediate results which are returned by one function and immediately consumed by another one.

## Design Patterns
### Model View Controller

### Singleton
The classes _Network_ and _HTMLParserFactory_ are singletons, as one of them is sufficient for the whole programme.

### Factory
_HTMLParserFactory_ produces parsers for the different HTML standards.

### Visitor
_RenderTreeNode_, _RenderTreeNodeVisitor_, and _RenderNode<HTML tags>_ implement the Visitor pattern.

### Observer
Each element in _View_ implements the observer pattern enabling the webbrowser to trigger functions if the user performs actions on the elements.


# Activity and Sequence Diagram
For Activity and Sequence Diagrams, we decided to focus on the essential actions that our browser should allow. We have 4 Activity Diagrams, namely:
- Refreshing the webpage
- Going to the previous page
- Accessing the URL

We omitted the "Going to the next page" Action Diagram, as this action is very similar to "Going to the previous page".

For each Action Diagram, we also designed a Sequence Diagram to illustrate the flow of an action with less abstraction from the actual code.

# Component Diagram





