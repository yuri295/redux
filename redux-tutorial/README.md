### Three Core Concepts

- store
  - holds the state of your application.
- action
  - describes the changes in the state of the application.
- reducer
  - actually carries out the state transition depending on the action.

### Three Principles

- The state of your whole application is stored in an object tree within a single store.

- The only way to change the state is to emit an action,an object describing what happened.

- To specify how the state tree is transformed by actions, you write pure reducers.
