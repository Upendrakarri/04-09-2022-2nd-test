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


## WHAT'S THE USE OF useMo() Hook

The useMemo is a hook used in the functional component of react that returns a memorized value.
In Computer Science, memoization is a concept used in general when we don’t need to recompute the function with a given argument for the next time as it returns the cached result.
A memoized function remembers the results of output for a given set of inputs.
FOR EXAMPLE , if there is a function to add two numbers, and we give the parameter as 1 and 2 for the first time the function will add these two numbers and return 3, but if the same inputs come again then we will return the cached value i.e 3 and not compute with the add function again.
In react also, we use this concept, whenever in the React component, the state and props do not change the component and the component does not re-render, it shows the same output. The useMemo hook is used to improve performance in our React application.


