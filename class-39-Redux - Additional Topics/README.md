

**Redux Toolkit (RTK):**
1. **Concerns Addressed:** Redux Toolkit simplifies Redux by reducing boilerplate code, handling immutability, providing easy reducer creation with `createSlice`, and managing async actions with `createAsyncThunk`.

2. **configureStore():** It configures a Redux store with defaults, making store setup easier.

3. **createSlice():** `createSlice` defines a Redux slice with initial state, reducers, and action creators in one place.

**MobX:**
1. **MobX:** It's a state management library for JavaScript and React that ensures consistent state by tracking changes in observable state, computed values, and triggering reactions.

2. **Consistency in MobX:** MobX maintains consistency by automatically updating derived values and UI components when observable state changes.

3. **Reactive UI:** To build a reactive UI with MobX, define observable state, create computed values, wrap components with `observer`, and modify state using MobX's `action` functions. This ensures your UI reacts to changes in data.