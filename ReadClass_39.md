# Reading Topics #39:


## REACT Context:

- React Context is a feature in React that provides a way to manage state and enables data sharing between components without having to pass props through all levels of the component tree. It allows you to create a global state that can be accessed by any component within a specific part of the component tree without explicitly passing it down as props.

React Context helps in managing state and data sharing in a React application by providing the following key components:

1. Context Provider: The Context Provider component wraps the entire subtree of components that need access to the shared data. It accepts a value prop, which represents the data that needs to be shared. All the components within the wrapped subtree can access this data.

2. Context Consumer (or useContext hook): The Context Consumer is used inside the components that need to access the shared data. It allows these components to consume the data provided by the Context Provider.

3. createContext: This function is used to create a new Context. It returns an object with two properties - Provider and Consumer (though Consumer can also be used with the useContext hook).

---
## useContext Hook:

The useContext hook is a built-in React hook that allows functional components to consume data from a React Context without the need for a Context Consumer component. 

1. Step 1: Create a new Context using createContext():
```
import { createContext } from 'react';

const AppContext = createContext();

export default AppContext;
```
Step 2: Wrap the relevant component subtree with the Context Provider:


```
import React from 'react';
import AppContext from './AppContext';
import ComponentA from './ComponentA';

const App = () => {
  const sharedData = { /* Your shared data here */ };

  return (
    <AppContext.Provider value={sharedData}>
      <ComponentA />
    </AppContext.Provider>
  );
};

export default App;
```
Step 3: Access the shared data in the nested component using the useContext hook:


```
import React, { useContext } from 'react';
import AppContext from './AppContext';
import ComponentB from './ComponentB';

const ComponentA = () => {
  const sharedData = useContext(AppContext);

  return (
    <div>
      {/* Use the shared data here */}
      <ComponentB />
    </div>
  );
};

export default ComponentA;
```

Step 4: Access the shared data in another nested component using the useContext hook:

```
import React, { useContext } from 'react';
import AppContext from './AppContext';

const ComponentB = () => {
  const sharedData = useContext(AppContext);

  return (
    <div>
      {/* Use the shared data here */}
    </div>
  );
};

export default ComponentB;
```

---

## Next.JS:

Next.js is a popular open-source framework for building React-based web applications. It is built on top of React and provides a set of features that simplify and enhance the development process. Next.js offers various benefits, such as server-side rendering (SSR), automatic code splitting, static site generation (SSG), and simplified routing, among others. Its primary purpose is to enable developers to build scalable and high-performance web applications with ease.

Example: Blog with Pagination

---