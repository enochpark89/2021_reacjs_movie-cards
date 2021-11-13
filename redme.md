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

