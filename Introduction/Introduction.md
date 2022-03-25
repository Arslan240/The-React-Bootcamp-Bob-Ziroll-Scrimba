

# Default Props
What are default props? We use default props as fallback prop values
If the props values are not passed in then our code will not break if we have 
default props values

# Props Types
  * We can also specify prop types. We have to 
    > `import PropTypes from 'prop-types'`
  * To assing propTypes we use simply the previous syntax and create an object then assign property to that object and we can assign string value or others
    > `Card.propTypes = { cardColor: PropTypes.string }`
  * These PropTypes will not show in deployed app, these are just development tools
  * We can also make a prop required by using `isRequired` with PropTypes like this -> `PropTypes.string.isRequired`
  * We can also chain properties, e.g if we are using functions then we use function first and then we assing any properties to it `PropTypes.oneOf(['blue', 'red', 'green']).isRequired`
  * `oneOf([])` is used for enum types

