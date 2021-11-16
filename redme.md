# ReactJS


# Introduction
- Introduction:

- Problem that reactJS is fixing.
- If you don't investigate what problems that it is fixing, the solution is not going to make sense. 
- Instead of memorizing, it is good to compare VanillaJS and ReactJS and he wants to sell me that ReactJs is so much better. 
- ReactJS can make interactivity in a super simple way.
- ReactJS team focuses on that. 
- reactJS theme knows this
- After you make a comparision, you will see how ReactJS improved so much on JavaScript. 
- Test by counting clicks app. 


# Before React

- Before React, you had to do so many things to create a counter

1. Create HTML 
2. Grab from javascript
3. Listen for event
4. Update data. 
5. Update your HTML tags.

- This is too repetitive. 

```html

```
- in order to call react, you have to import two URL. 
URL1:https://unpkg.com/react@17.0.2/umd/react.production.min.js
URL2:https://unpkg.com/react-dom@17.0.2/umd/react-dom.production.min.js
- 

# 2.3 Events in React

- React.createElement("<name of an element>", <EventListeners>, <content of the button>): This will create an element. 
- ReactDOM.render(<put multiple components>).
- Benefit: with one statement, you can create the element, an eventListener, and set the value.

# 2.5 JSX

- There is a easier way to create an element. you can use jsx.
```jsx
const Title = <h3 id="title" onMouseEnter={() => console.log("mouse enter)}>Hello I'm a title</h3>
```
- if you want to use this, you need to install babel because it will translate JSX to html
URL:
https://unpkg.com/@babel/standalone/babel.min.js

- To include button
- example:

1. make them into a function
```js
const Title = () => {
    return(<event hander> + <functions>);
}
```
2. Include the function into the component

```jsx
const Container = () => (
<div>
    <Title />
</div>
);
// render them to the HTML page.
ReactDOM.render(<Container />, root);
```


*Make sure to make the function that you are including or styled-Component into an uppercase*

# 3.0 Understanding State

- State can replace updating the data in JavaScript
- NOT SO GOOD WAY:
```js
let counter = 0;

// CountUP() Will rerender the webpage with render() function because HTML needs to change along with data.
function CountUp() {
    counter = counter+1;
    render()
}

function render() {
    ReactDOM.render(<Continer />, root);
}

// include variable in JSX
const Containter = () => (
    // If you change the counter, it will change the jsx and then html.
    <div>
        <h3>Total clicks: {counter} </h3>
        <button onClick={CountUp}>Click me </button>
    </div>
)
ReactDOM.render(<Continer />, root);
```
- This will not update the counter from the HTML because the state is only running once.
- We are not running a state or we are not rerendering the webpage again.
- If you rerender it it will work. 

- when you check the elements with the Chrome Dev Tool, you will see the HTML getting updated everytime. 
- React JS only changes the part that need to be changed.

# 3.1.  setState - Part One

- PROFESSIONAL WAY:
```js
```
