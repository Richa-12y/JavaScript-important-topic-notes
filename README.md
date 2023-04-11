# JavaScript-important-topic-notes

## Arrow function
 ###  Arrow function is alternet to traditional function Expression.

 > There are some limitations on Arrow function
- Arrow function dont't have there own bindings to `this`, `arguments`, or `super`, and should not be used as methods.
- Arrow function can't be used as `constructors`. Calling them with new throws a `TypeError`. They also don't have access to the `new.target keyword`.
- Arrow functions cannot use `yield` within their body and cannot be created as `generator functions`.
