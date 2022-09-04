## WHAT ARE COMPONENTS IN REACT

components are reusable class/functions which contains the JSX.
One file can have multiple classes/function, therefore it can have multiple components.
components can return the JSX.
Components have to be exported.
To maintain cleaner code structure. We create a directory called as components inside the src.
The Component name should follow PascalCasing. Otherwise it will not work.
Inside components we put all the various components that we will be using.


## WHAT ARE PROPS IN REACT

Props means sending of data from one component to another component.
Typically it is Parent to child.
In the Parent, we send as an attribute. (Because in the parent, we write HTML like syntax and in HTML, the way we send any data to the element is using attributes).
In the child component. For functional component, we can get the prop directly as the function's parameter.
The Props only flows from parent to Child Component.
The prop data can be anything, primitive data type, non primitive data type, even functional references.
