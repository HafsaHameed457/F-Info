##  What is ReactJS?
ReactJS is a JavaScript library used to build reusable components for the view layer in MVC architecture. It is highly efficient and uses a virtual DOM to render components. It works on the client side and is written in JSX.

## Important Features of React:

1. Virtual DOM: React uses a virtual DOM to efficiently update and render components, ensuring fast performance by minimizing direct DOM manipulations.
2. Component-Based Architecture: React builds UI using reusable, isolated components, making code more modular, maintainable, and scalable.
3. Hooks: React hooks allow functional components to manage state and side effects, making them powerful and more flexible.


## Explain the MVC architecture.

The Model-View-Controller (MVC) framework is an architectural/design pattern that separates an application into three main logical components Model, View, and Controller. Each architectural component is built to handle specific development aspects of an application. It isolates the business, logic, and presentation layer from each other

## Explain the building blocks of React.

Components: These are reusable blocks of code that return HTML.
JSX: It stands for JavaScript and XML and allows you to write HTML in React.
Props and State: props are like function parameters and State is similar to variables.
Context: This allows data to be passed through components as props in a hierarchy.
Virtual DOM: It is a lightweight copy of the actual DOM which makes DOM manipulation easier.

## Explain props and state in React with differences

Props are used to pass data from one component to another. The state is local data storage that is local to the component only and cannot be passed to other components.

## What is virtual DOM in React?

The Virtual DOM in React is an in-memory representation of the actual DOM. It helps React efficiently update and render the user interface by comparing the current and previous virtual DOM states using a process called diffing.

## How Virtual DOM Works

Efficient Rendering: The Virtual DOM is an in-memory representation of the actual DOM that React uses to optimize the process of updating and rendering UI changes.
Diffing Algorithm: React compares the current and previous versions of the Virtual DOM using a diffing algorithm, identifying the minimal set of changes required to update the real DOM.
Batch Updates: Instead of updating the real DOM immediately, React batches multiple changes to reduce unnecessary re-renders, improving performance.
Faster Updates: Since updating the real DOM is slow, React minimizes direct DOM manipulations by only making updates where necessary after comparing the Virtual DOM.
Declarative UI: With the Virtual DOM, React allows developers to write code in a declarative style, letting React handle when and how to efficiently update the UI.

## What is JSX?

JSX is basically a syntax extension of regular JavaScript and is used to create React elements. These elements are then rendered to the React DOM. All the React components are written in JSX. To embed any JavaScript expression in a piece of code written in JSX we will have to wrap that expression in curly braces {}. 

## What are components and their type in React?
A Component is one of the core building blocks of React. In other words, we can say that every application you will develop in React will be made up of pieces called components. Components make the task of building UIs much easier. 

 In React, we mainly have two types of components: 

Functional Components: Functional components are simply javascript functions. We can create a functional component in React by writing a javascript function. 

Class Components: The class components are a little more complex than the functional components. The functional components are not aware of the other components in your program whereas the class components can work with each other. We can pass data from one class component to another class component.

## How do browsers read JSX?

In general, browsers are not capable of reading JSX and only can read pure JavaScript. The web browsers read JSX with the help of a transpiler. Transpilers are used to convert JSX into JavaScript. The transpiler used is called Babel.

## How to create an event in React?

To create an event in React, attach an event handler like onClick, onChange, etc., to a JSX element. Define the handler function to specify the action when the event is triggered, such as updating state or executing logic.

## What is a key in React?

A “key” is a special string attribute you need to include when creating lists of elements in React. Keys are used in React to identify which items in the list are changed, updated, or deleted. In other words, we can say that keys are used to give an identity to the elements in the lists.

## Explain the use of render method in React?

React renders HTML to the web page by using a function called render(). The purpose of the function is to display the specified HTML code inside the specified HTML element. In the render() method, we can read props and state and return our JSX code to the root component of our app.

## What is state in React?
The state is an instance of React Component Class that can be defined as an object of a set of observable properties that control the behaviour of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.

## Explain props in React?

React allows us to pass information to a Component using something called props (which stands for properties). Props are objects which can be used inside a component

## What is higher-order component in React?

Higher-order components or HOC is the advanced method of reusing the component functionality logic. It simply takes the original component and returns the enhanced component. HOC are beneficial as they are easy to code and read. Also, helps to get rid of copying the same logic in every component.

## Functional vs class components

A functional component is just a plain JavaScript pure function that accepts props as an argument 	A class component requires you to extend from React. Component and create a render function 
No render method used	It must have the render() method returning JSX 
Also known as Stateless components 	Also known as Stateful components
React lifecycle methods (for example, componentDidMount) cannot be used in functional components.	React lifecycle methods can be used inside class components (for example, componentDidMount).
Constructors are not used.	Constructor is used as it needs to store state. 

## Explain one way data binding in React?

ReactJS uses one-way data binding which can be Component to View or View to Component. It is also known as one-way data flow, which means the data has one, and only one way to be transferred to other parts of the application. In essence, this means child components are not able to update the data that is coming from the parent component. It is easy to debug and less prone to errors.

-- Intermediate qs --

## What is conditional rendering in React?

Conditional rendering in React involves selectively rendering components based on specified conditions. By evaluating these conditions, developers can control which components are displayed, allowing for dynamic and responsive user interfaces in React applications.

## What is react router?

React Router is a standard library for routing in React. It enables the navigation among views of various components in a React Application, allows changing the browser URL, and keeps the UI in sync with the URL.

## Explain the components of a react-router

The main components of a react-router are:

Router(usually imported as BrowserRouter):  It is the parent component that is used to store all of the other components. Everything within this will be part of the routing functionality
Switch: The switch component is used to render only the first route that matches the location rather than rendering all matching routes.
Route: This component checks the current URL and displays the component associated with that exact path. All routes are placed within the switch components.
Link: The Link component is used to create links to different routes.

