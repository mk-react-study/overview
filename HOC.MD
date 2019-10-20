# HOC

- Convention to start name hoc component `With` 
- Pourpose of HOC is to add common functionality to component.

### Example HOC
- Dummy Hoc

```
const aux = props => props.children;
export default aux;
```

- Applying common logic to component 
```
import React from 'react';
const withClass = props => (
  <div className={props.classes}>{props.children}</div>
);
export default withClass;
```

```
return (
      <WithClass classes={classes.App}>
        <button
          onClick={() => {
            this.setState({ showCockpit: false });
          }}
        >
      </WithClass>
    );
```

- Passing component in HOC
```
import React from 'react';
const withClass = (WrappedComponent, className) => {
  return props => (
    <div className={className}>
      <WrappedComponent {...props}/>  {/* this allow to pass props to next level. */}
    </div>
  );
};
export default withClass;
```

```
class App extends Component {
  render() {
    return (
      <Aux/>
    );
  }
}
export default withClass(App, classes.App);
```
// Here withClass is not component by itself, it returns component, That's why name started with small letter


