# JavaScript-important-topic-notes

## Arrow function
 ###  Arrow function is alternet to traditional function Expression.

 > There are some limitations on Arrow function
- Arrow function dont't have there own bindings to `this`, `arguments`, or `super`, and should not be used as methods.
- Arrow function can't be used as `constructors`. Calling them with new throws a `TypeError`. They also don't have access to the `new.target keyword`.
- Arrow functions cannot use `yield` within their body and cannot be created as `generator functions`.

### code example

`const callData = (a) => {
  if (a % 2 === 0) {
    return Promise.resolve({
      message: "hey you are even number",
    });
  } else {
    return Promise.reject("not even");
  }
};`


// callData(4)
//   .then((c) => console.log(c))
//   .catch((c) => console.log(c))
//   .finally(() => console.log("task done"));

`const getResult = async () => {
  try {
    let result = await callData(2);
    console.log(result);
  } catch (e) {
    console.log(e);
  }
};`

`getResult()`;

