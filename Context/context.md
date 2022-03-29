# React Context
  * Context is used to solve the problem of props drilling to the very bottom of component tree in react.
  * We use `React.createContext()` which creates a new context and returns a themecontext.
  * This themecontext contains `Provider` and `Consumer`. 
  * The provider is the component which contains the state, and the consumer are the components which needs those state down the tree somewhere.
  * This context stuff only works on class components, not on functional components

# ThemeContext.Provider
  >`<ThemeContext.Provider value={"dark"}>
  >   <App />
  > </ThemeContext.Provider>`

  

# ThemeContext.Consumer
  >`<ThemeContext.Consumer>
  >   {theme => ( 
  >     <Button theme={theme} />
  >   )}
  > </ThemeContext.Consumer>`

  * This .consumer tag is wrapping the button component, this is according to the pattern of passing the render props as children. 
  * In children we can also pass callback function which accepts actually the value which is being distributed to all the child components by the provider.
  * We can pass that value to the consumer.