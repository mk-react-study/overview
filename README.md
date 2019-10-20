# Overview
## Some Use full npm 
-   https://www.npmjs.com/package/shortid
```
import shortId from 'shortid'
let requestSessionId = shortId()
```
- https://www.npmjs.com/package/prop-types
```
import React from 'react';
import PropTypes from 'prop-types';
class MyComponent extends React.Component {
  render() {
    // ... do things with the props
  }
}
 
MyComponent.propTypes = {
  // You can declare that a prop is a specific JS primitive. By default, these
  // are all optional.
  optionalArray: PropTypes.array,
  optionalBool: PropTypes.bool,
  optionalFunc: PropTypes.func
}
```
- https://www.npmjs.com/package/moment
- https://www.npmjs.com/package/mobx
- https://www.npmjs.com/package/react-router-dom
- https://www.npmjs.com/package/react-moment
- https://www.npmjs.com/package/cookie-cutter
- https://www.npmjs.com/package/jwt-decode
- https://www.npmjs.com/package/axios
- https://www.npmjs.com/package/nodemon
- https://www.apollographql.com/docs/
- https://www.npmjs.com/package/unstated
- https://bootswatch.com/  This is for themes
```
Add this in index.html
Change title in index.html
```
- Install Apollo Client for grapql https://www.apollographql.com/docs/react/get-started/
```
npm install apollo-boost @apollo/react-hooks graphql
```
- https://www.npmjs.com/package/cors  `Allow cross-origin`
```
const express = require('express')
const cors = require('cors')
const app = express()
app.use(cors())
```

- If New State is depended of old state, then use 
```
this.setState((prevState, props) => {
  return {
    persons: persons,
    changeCounter: prevState.changeCounter + 1
  };
});
```
Because setState is not immediately update the state, it is request to react, but prevState provide update correct value.
```
this.setState(
  {
    persons: persons,
    changeCounter: this.changeCounter + 1
  });

```

