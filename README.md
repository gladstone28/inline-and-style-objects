[Link to codecademy lesson](https://www.codecademy.com/courses/react-101/lessons/react-style/exercises/inline-styles-and-style-object-variables)


### React Styles
**Inline Styles and Style Object Variables**


There are many different ways to use styles in React. This exercise is focused on two of them: inline styles and style object variables.

An inline style is a style that’s written as an attribute, like this:
```
<h1 style={{ color: 'red' }}>Hello world</h1>
```
Notice that it has double curly braces. The outer curly braces are to note that everything between should be read as JavaScript. The inner curly braces create a JavaScript object literal.

However, using inline styles can quickly become messy if you want to apply more than just a few styles. An alternative is to store a style object in a variable and then inject that variable as the value of the style attribute.

To do this, we can initialize an object with properties and values like so:
```
const darkMode = {
  color: 'white',
  background: 'black'
};
```
Then, the object can be injected to style a component:
```
<h1 style={darkMode}>Hello world</h1>
```
Instructions

Checkpoint 1 Passed

1.    Let’s practice styling components using both inline styles and style object variables.

Open StyleDemo.js. Starting with inline styling, style the first <h1> element inside the StyleDemo component.

Give the <h1> element an attribute with the name of style. The attribute’s value should evaluate to this object:
```
{ background: 'lightgreen', color: 'darkgreen' }
```

Remember to surround the JavaScript object containing CSS styles with another pair of curly braces.

2. Next, let’s style using a style object variable.

On a new line, declare a new constant named myStyle. Set myStyle equal to this object:
```
{
  background: 'lightblue',
  color: 'darkblue'
}
```
Here’s an example of a JavaScript object called animal:
```
const animal = { name: "Black Bear", species: "Ursus Americanus" };
```
Style the second <h1> element by giving it an attribute with the name of style. The attribute’s value should be myStyle.
