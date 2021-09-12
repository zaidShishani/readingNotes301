# React: Component Lifecycle Events


## Reading questions :
1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’ ?

   reder since the mounting phase occur  in this order ( Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount)

2. What is the big difference between props and state?

    the differnce comesin how they are handled, props get controlled outisde of a component while state get controlled inside of a component.

3. When do we re-render our application?

    any time we update the component it will be rerendered for example in ***componentDidMount()*** when we call ***setState()*** and used sparingly it will cause a rerender, which can lead to perfomance issues and in ***shouldComponentUpdate()*** sicne the default behavior in react is to rerender after every state change.

4. What are some examples of things that we could store in state? 

    we store changes in values to to rerender the application wit the new value