# redux-persistate

### Installation

```bash
npm i -S redux-persistate
```

### Usage

**Save state**

```js
import { saveState } from 'redux-persistate'

store.subscribe(() => {
  saveState({user : store.getState().user})
})
```

**Load state**

```js
import { loadState } from './lib/localStorage'

const defaultState = loadState()
export const store = createStore(rootReducer, defaultState)
```
