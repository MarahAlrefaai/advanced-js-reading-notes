hooks ? 
Hooks are an experimental proposal to React. You don’t need to learn about them right now. Also, note that this post contains my personal opinions and doesn’t necessarily reflect the positions of the React team.


Why Hooks?
We know that components and top-down data flow help us organize a large UI into small, independent, reusable pieces. However, we often can’t break complex components down any further because the logic is stateful and can’t be extracted to a function or another component. Sometimes that’s what people mean when they say React doesn’t let them “separate concerns.”
These cases are very common and include animations, form handling, connecting to external data sources, and many other things we want to do from our components. When we try to solve these use cases with components alone, we usually end up with:
Huge components that are hard to refactor and test.
Duplicated logic between different components and lifecycle methods.
Complex patterns like render props and higher-order components.




Do Hooks Make React Bloated?
Before we look at Hooks in detail, you might be worried that we’re just adding more concepts to React with Hooks. That’s a fair criticism. I think that while there is definitely going to be a short-term cognitive cost to learning them, the end result will be the opposite.
If the React community embraces the Hooks proposal, it will reduce the number of concepts you need to juggle when writing React applications. Hooks let you always use functions instead of having to constantly switch between functions, classes, higher-order components, and render props.
