# Front-end-interview (React)

## Redux
Redux is a state management library for JavaScript apps. It helps manage the application's state in a predictable and centralized way, especially in large applications.

## Key Concepts of Redux

1. State:
 The entire application’s state is stored in a single object called the store.

 Think of it as the "brain" of your app.

2. Actions:
 Actions are plain JavaScript objects that describe what happened in the app.

 They must have a type field (e.g., 'ADD_TODO') and can optionally have additional data (payload).

3. Reducer:
 Reducers are pure functions that take the current state and an action, and return a new state.

 They specify how the state should change in response to an action.

4. Store:
 The store holds the state and provides methods to access it (getState), update it (dispatch), and  listen for changes (subscribe).

5. Selectors in Redux
 Selectors are functions that are used to extract or derive specific pieces of state from the Redux store. They help keep the code organized and reusable.

 Selectors can be used to get the state, manipulate it, or even compute derived values without directly modifying the store.

6. Subscription
 Components subscribe to the store to get updates whenever the state changes.

 Whenever the reducer updates the state, the store notifies the subscribers.


### Flow Summary in Code

 Create Store: Use createStore with a reducer.

 Dispatch Actions: Send actions using dispatch().
 
 Reducer Updates State: Based on the action’s type and payload.
 
 Get New State: Components react to the updated state

### Memoized Selectors (Re-Select)

For more advanced use cases, you can use libraries like reselect to create memoized selectors. These selectors cache their results and only recompute when the state they depend on changes. This can improve performance in large apps by avoiding unnecessary recalculations.

### Why Use Selectors?
Encapsulation: Selectors allow you to encapsulate the logic for extracting data, which keeps your components cleaner.

Reusability: You can reuse selectors across different parts of your app.

Performance: Selectors can be optimized to prevent unnecessary recalculations of derived state (using memoization).

## Redux-Saga
Redux-Saga is a middleware library for handling side effects (e.g., API calls, delays, or accessing browser storage) in a Redux application. It uses generators (a special type of JavaScript function) to make async flows more readable and maintainable.

## Why Use Redux-Saga?
Centralized Side Effect Management: Keeps all your async operations in one place.
Improved Readability: Generator functions make async code look synchronous.
Powerful Effects: Built-in effects like call, put, and takeEvery make handling complex flows easy.