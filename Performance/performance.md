# shouldComponentUpdate()
  * This is a method based on which react renders or not renders the component. This returns true or false.
  * It receives two arguments `nextProps` and `nextState`. Now based on this we can check if there has been any change in the state and return true. It'll rerender the component.
  * This works according to shallow comparison and can't really easily compare the values of prev and next states.

# React.pureComponent
  * It is a class which is replacement of `Component` class. This class automatically implements `shouldComponentUpdate()` for us and it actually warns us if we try to implement it by ourselves.
  * We have to extend all of our classes with PureComponent for this to work.
  * Using this will allows us to only render the components which are actually changing.