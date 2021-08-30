## Lists and Keys

Showing a list of elements happened almost in every project I was ever writing. And React really simplifies the rendering of lists inside the JSX by supporting the Javascript .map() method.

The .map() method in Javascript iterates through the parent array and calls a function on every element of that array. Then it creates a new array with transformed values. It doesn’t change the parent array.

Now, let’s imagine that you are creating a simple Todo App. The main element of your project will be a list of tasks. To show them, you will need data, which in most cases will be an array of elements, can be objects or strings, for example.

While you have the array with data, you can use the .map() method inside the JSX component the transform the data into the element.

## spread operator

The spread operator is a new addition to the set of operators in JavaScript ES6. It takes in an iterable (e.g an array) and expands it into individual elements.

The spread operator is commonly used to make shallow copies of JS objects. Using this operator makes the code concise and enhances its readability.

```
let baked_desserts = ['cake', 'cookie', 'donut'];
let desserts = ['icecream', 'flan', 'frozen yoghurt', ...baked_desserts];
console.log(desserts);
//Appending baked_desserts after flan
let desserts2 = ['icecream', 'flan', ...baked_desserts, 'frozen yoghurt'];
console.log(desserts2);

```