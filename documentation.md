# Class diagramme

## Constructors, Getters, and Setters
For the sake of brevity and in order to keep the UML as compact as possible we decided just to mention Constructors, if they are somehow "special", otherwise we don't mention them in the class diagram. Furthermore, we made most of our variables private, but didn't specifically created Getters and Setters as methods, as this would blow up the class diagramms unnecessarily.

## Classes and strukts without connections
Some of our classes and structs are not connected to any other class. The reason for that is, that they are never "stored" or kept as a state anywhere in the programme, but are just temporary intermediate results which are returned by one function and immediately consumed by another one.

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
We have 4 activity diagrams namely:
- Initializer
- Refreshing the webpage
- Going to the previous page
- Accessing the URL

We omitted the action "Going to the next page" as this action is very similar to "Going to the previous page".
For each action diagram we also designed a sequence diagram.


# Components





