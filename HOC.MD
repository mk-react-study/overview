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
