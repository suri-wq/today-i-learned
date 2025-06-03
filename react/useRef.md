# useRef

A React hook used to reference a value that persists across renders **without causing re-renders**. It's commonly used for accessing DOM elements or storing mutable values that shouldn't trigger updates to the UI.



## Syntax

```js
const ref = useRef(initialValue)
```

## Use Cases


### 1. Accessing a DOM Element

```js
import { useRef, useEffect } from "react"

function App() {
    const inputRef = useRef(null)

    useEffect(() => {
        inputRef.current.focus()  // Automatically focus the input on mount
    }, [])

    return <input ref={inputRef} placeholder="Focus me!" />
}
```

### 2. Storing values that persist across renders but don’t cause re-renders

```js
const countRef = useRef(0)

function handleClick() {
    countRef.current += 1
    console.log("Clicked", countRef.current, "times")
}
```