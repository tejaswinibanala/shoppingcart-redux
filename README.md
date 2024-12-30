**About Redux**

**What is Redux?**
Redux is a predictable state management library often used in React applications. It helps manage the state of your app in a centralized store, simplifying the handling and debugging of data flow, especially as your application scales in complexity.

**Key Concepts of Redux:**
**Store:**
The single source of truth for the application's state. It holds the entire state tree.

**Actions:**
Plain JavaScript objects that describe what needs to happen (e.g., "add item to cart," "remove item from cart"). Actions consist of a type and an optional payload for extra data.

**Reducers:**
Pure functions that specify how the application's state changes in response to actions. A reducer takes the current state and an action, returning a new state.

**Dispatch:**
A method used to send actions to the store, triggering reducers to compute and update the state.

**Selectors:**
Functions that extract specific data slices from the store, allowing components to use and react to state changes.

**Why Redux?**
**Centralized State**: All app states reside in one place, ensuring consistency and easier debugging.
**Predictability:** Changes to state follow predictable, testable patterns through actions and reducers.
**Time-Travel Debugging:** Tools like Redux DevTools allow tracking, rewinding, or replaying state changes.
**Scalability:** Efficient state organization supports complex applications.

**How Redux Works in the Shopping Cart App:**
**Store:**
Maintains application data, such as the list of cart items and total price.

**Actions:**

add: Adds an item to the cart.
remove: Removes an item from the cart.

**Reducers:**
Define how the cartList and total fields update based on dispatched actions.

Dispatch:
Actions are dispatched when users click buttons like "Add to Cart" or "Remove", triggering state updates.

Selectors:
Components subscribe to the state and display relevant slices like the current cart items or the total price.

Redux Toolkit
This project uses Redux Toolkit, a modern, streamlined approach to Redux development. Redux Toolkit provides tools like createSlice, which reduces boilerplate by combining reducers, actions, and state into a single function.

Using Redux Toolkit makes it simpler to configure the store and ensures clean, maintainable code for efficient state management.







