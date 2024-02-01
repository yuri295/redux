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

### Async actions

- state
  - loading: Display a loading spinner in your component
  - data: List of users
  - error: Display error to the user
- actions
  - FETCH_USERS_REQUEST: Fetch list of users
  - FETCH_USERS_SUCESS: Fetched successfully
  - FETCH_USERS_FAILURE: Error fetching the data
- reducers
  - case: FETCH_USERS_REQUEST
    loading: true
  - case: FETCH_USERS_SUCESS
    loading: false
    users: data (from API)
  - case: FETCH_USERS_FAILURE
    loading: false
    error: error (from API)

### Async action creators

- axios: Request to an API and point
- redux-thunk: Define async action creators, middleware
