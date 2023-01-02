### Conceptual Exercise

Answer the following questions below:

- What are some ways of managing asynchronous code in JavaScript?

- What is a Promise?
  a value represented by either Resolve, Rejected, or pending when accessing API's.

- What are the differences between an async function and a regular function?
  A sync Functions will prevent JS from proceeding till the async function is completed. Without it, JS will skip on to the next function.

- What is the difference between Node.js and Express.js?
  Node is server sided javascript and express is a web aplication library that works with javascript. 

- What is the error-first callback pattern?

- What is middleware?

- What does the `next` function do?
  allows async functions to proceed to the next function prior to completing. 

- What are some issues with the following code? (consider all aspects: performance, structure, naming, etc)

```js
async function getUsers() {
  const elie = await $.getJSON('https://api.github.com/users/elie');
  const joel = await $.getJSON('https://api.github.com/users/joelburton');
  const matt = await $.getJSON('https://api.github.com/users/mmmaaatttttt');

  return [elie, matt, joel];
}
```
const should be "let"

