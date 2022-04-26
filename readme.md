
React and JavaScript Interview Questions and Answers:

- 1.<a href="ReactInterviewQuestions.md">React Interview Questions</a>

- 2.<a href="JavaScriptInterviewQuestions.md">JavaScript Interview Questions</a>

Some React Interview Questions:

# What is Babel?
=> Babel is a JavaScript compiler that includes the ability to compile JSX into regular JavaScript.

# What is React? Explain in detail its uses, why we need to use  it, what are some features, when was it made and what are some alternatives?
=> React allows developers to create large web applications that can change data, without reloading the page. The main purpose of React is to be fast, scalable, and simple. It works only on user interfaces in the application. This corresponds to the view in the MVC template.

Some of the important features of ReactJS are:
 - Components. 
 - JSX.
 - Virtual DOM.
 - One-way Data Binding.
 - Performance
 - Simplicity.

React was created by Jordan Walke, a software engineer at Facebook, who released an early prototype of React called "FaxJS". He was influenced by XHP, an HTML component library for PHP. It was first deployed on Facebook's News Feed in 2011 and later on Instagram in 2012. It was open-sourced at JSConf US in May 2013.

The most popular alternatives and competitors to React are:
- Angular 2, 
- Vue. js, 
- Ember. js, 
- NativeScript, and 
- jQuery 

# What is Webpack?
=> Webpack is a static module bundler for JavaScript applications — it takes all the code from your application and makes it usable in a web browser. Modules are reusable chunks of code built from your app's JavaScript, node_modules, images, and the CSS styles which are packaged to be easily used in your website.

# What is setState?
=> setState() setState(updater, [callback]) setState() enqueues changes to the component state and tells React that this component and its children need to be re-rendered with the updated state. This is the primary method you use to update the user interface in response to event handlers and server responses.

# What is Virtual DOM?
=> React uses Virtual DOM exists which is like a lightweight copy of the actual DOM(a virtual representation of the DOM). So for every object that exists in the original DOM, there is an object for that in React Virtual DOM. It is exactly the same, but it does not have the power to directly change the layout of the document. Manipulating DOM is slow, but manipulating Virtual DOM is fast as nothing gets drawn on the screen. So each time there is a change in the state of our application, virtual DOM gets updated first instead of the real DOM.

# What are React Portals?
=> React portals provide a first-class way to render and allow child components, which are typically present outside the DOM, to live within a Document Object Model (DOM) node. This React portal component exists outside the DOM hierarchy of the parent component.
```js
ReactDOM.createPortal(child, container)
```
# What is context API?
=> The Context API is a React structure that enables you to exchange unique details and assists in solving prop-drilling from all levels of your application.

# What are Life cycle methods in React?
=> Each component in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting.

# Explain ComponentDidMount, ComponentDidUpdate, => ComponentWillUnmount?
=>The componentDidMount() : invoked immediately after a component is mounted (inserted into the DOM tree).
The componentDidUpdate(prevProps, prevState, snapshot) : is invoked immediately after updating occurs. This method is not called for the initial render.
The componentWillUnmount() method allows us to execute the React code when the component gets destroyed or unmounted from the DOM (Document Object Model). This method is called during the Unmounting phase of the React Life-cycle i.e before the component gets unmounted.

# Explain useEffect, useState API in biref?
=> The useEffect Hook allows you to perform side effects in your components. Some examples of side effects are: fetching data, directly updating the DOM, and timers. useEffect accepts two arguments. The second argument is optional. useEffect(<function>, <dependency>).

useState is a Hook that allows you to have state variables in functional components. You pass the initial state to this function and it returns a variable with the current state value (not necessarily the initial state) and another function to update this value.

# How can you memoize components in React?
=> Components using hooks can be freely wrapped in React. memo() to achieve memoization. React always re-renders the component if the state changes, even if the component is wrapped in React.

To implement memoization in a class component, we'll use React. PureComponent. React. PureComponent implements shouldComponentUpdate(), which does a shallow comparison on state and props and renders the React component only if there's a change in the props or state.
