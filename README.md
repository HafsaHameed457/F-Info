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
The store holds the state and provides methods to access it (getState), update it (dispatch), and listen for changes (subscribe).

5. Selectors in Redux
Selectors are functions that are used to extract or derive specific pieces of state from the Redux store. They help keep the code organized and reusable.

Selectors can be used to get the state, manipulate it, or even compute derived values without directly modifying the store.