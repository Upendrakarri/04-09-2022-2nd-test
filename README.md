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


## How to use css in react

There are three ways to attach styling.
External CSS -> Using index.css

body{
  background-color: blueviolet;
}

button{
  background-color: brown;
}
h2{
  background-color: aqua;
}

Index.css is imported at index.js level, therefore it is available pretty much everywhere.



Modular CSS -> For every module, we will have a css.

import '../App.js';
function MyArrayComp (props) {
    console.log(props);
    return (
        <h2>2nd week test</h2>
    )
}
export default MyArrayComp;


The idea is better code organization.
For each module, we will have it's relevant css file.
This keep the code files organized and structured.
Instead of having 1 very large file, we have more files but smaller in size comparatively.


Third Approach: Inline styling.


const style = {
    color: "yellow", 
    backgroundColor: "blue"
  };
  return (
    <div>
      <h2>using index.css</h2>
      <MyComponents caption="click here"/>
      {/* <MyComponents caption="BUTTON 2"/> */}
      {/* <MyComponents caption="BUTTON 3"/> */}
      <br/>
      <MyArrayComp abcd_arr={arr}/>
      <p style={style}>using Inline css</p>
      
      

In the same like we give the style attribute.
This attribute is actually an object.

