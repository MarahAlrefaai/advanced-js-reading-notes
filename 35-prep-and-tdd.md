In this comprehensive tutorial, Dan Abramov - the creator of Redux - will teach you how to manage state in your React application with Redux.

State management is absolutely critical in providing users with a well-crafted experience with minimal bugs.

It's also one of the hardest aspects of a modern front-end application to get right.

Redux provides a solid, stable, and mature solution to managing state in your React application. Through a handful of small, useful patterns, Redux can transform your application from a total mess of confusing and scattered state, into a delightfully organized, easy to understand modern JavaScript powerhouse.

The principles of Redux aren't new, but they are packaged and presented for you in an easy to use a library that not only elevates your applications but also improves your general understanding of building JavaScript UIs.

In this course, Dan Abramov will show you the fundamentals of Redux, so that you can start using it to simplify your applications.



Reducers
Just a quick refresher on what reducer is before we go into testing and code. Redux documentation is still great, in fact it covers unit tests really well you don’t even have to read this post. To summarize it, the reducer is a pure function that takes the previous state and an action, and returns the next state.


Pure functions
Because it’s a pure function, it’s easy to test. It’s a function that produces no side effects; given the same input, will always return the same output; doesn’t rely on external state.

What to test
Usually reducer consists of initial state and switch statement to handle every action. I like to break down my store into different sub-stores and have separate reducers for each sub-store. Sometimes one switch/case may handle few actions, because the business logic is the same and outcome should be the same. Some example GET_POST and UPDATE_POST should update the same store and produce same outcome.

It’s important to test reducers. That’s where business logic should happen and where new application state is formed based on external (API) or internal response.
