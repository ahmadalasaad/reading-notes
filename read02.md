## React lifecycle

What are component lifecycle events?

React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. 

These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

### constructor()

The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. constructors can be used to assign state using this.state or to bind event handle methods to an instance. Let’s take a look at some example code.

### static getDerivedStateFromProps()

This method exists for rare cases where the state relies on changes in props over time.

### render()

Render is the only required method in a class component. It will examine this.props and this.state when called. The render function should not modify the component state because it would cause a lot of bugs by changing the state every time it rerenders. I also should not directly interact with the browser. render will not be invoked if shouldComponentUpdate() returns false. Here is an example of using render.

### componentDidMount()

This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().


## React State Vs Props

### What types of things can you pass in the props?

The values can be any data type, from strings to functions, objects, etc.


### What is the big difference between props and state?

The key difference between props and state is that state is internal and controlled by the component itself while props are external and 

controlled by whatever renders the component

### When do we re-render our application?

React components automatically re-render whenever there is a change in their state or props.

### What are some examples of things that we could store in state?

form,counter,etc