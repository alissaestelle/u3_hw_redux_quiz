# Redux Quiz

<img src="https://chriscourses.com/img/blog/redux/redux.jpg" height="400px"/>

## Getting Started

- Fork and Clone

## Questions

1. What is Redux?

```
Redux is a library that allows state to be stored nonlinearly. It stores state collectively and uses a reducer (switch statement) to determine which state to use.
```

2. What packages do we install to use Redux?

```
Redux requires three packages: react-redux, redux, and redux-devtools-extension.
```

3. In your own words, describe the flow of how Redux is used to manage state.

```
Redux uses actions, types, and reducers to manage flow state. Reducers are used to compartmentalize state, actions determine how state performs, and types define the type of action being performed.
```

4. What do we use in order to manage different pieces of state?

```
Reducers are used to manage state.
```

5. What do we use to perform an update to state?

```
Actions are used to update state.
```

6. How do we access state from Redux?

```
State is accessed by type (i.e. action.type within the reducer)
```

7. In your own words, describe how to set up Redux for a React App.

```
1. Install React Redux dependencies (react-redux, redux, and redux-devtools-extension).
2. Inside the src folder, create a store folder. Inside the store folder, build the main Redux folder structure: an actions folder, a reducers folder, a types.js file, and a store/index.js file.
3. Enable the Redux Store within store/index.js, then export the new store variable and import it into React's index.js, along with React's Provider component. Wrap <Provider> around <App>, add a prop to <Provider> and assign the imported store variable as its value.
4. Define types and actions in their respective folders/files. Import any type variables (from types.js) into an actions/file.js and  create any necessary action functions, each fx containing an object with two keys: type and payload. Assign each imported type variable as a value to its relative type key (type values correspond to the fx name). Define parameters for payload keys as well.
5. Import types variables (again) into a reducers/file.js. Create an initial state variable and a reducer fx containing a switch statement. Use the imported types variables as switch cases (each returning specific actions/payloads).
6. In store/index.js, tie everything together by importing { composeWithDevTools }, { combineReducers } (in cases where there are multiple), and any reducer functions. Create keys to represent reducer states and assign the reducer functions as values within the store variable (originally created in step two)
7. Import { connect } into a new React component as well as any action functions (or other components), then create two functions to dispatch actions: mapStateToProps() and mapActionsToProps().


```

## Submission

Pull Request due by **9AM EST** following the [PR Submission Guidelines](https://github.com/SEI-R-2-22/template_pull_request).
