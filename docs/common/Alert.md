# Alert

### Props
1. **anchorOrigin** - (not required) position of the alert
```
anchorOrigin?: {
    vertical: "top" | "bottom";
    horizontal: "left" | "center" | "right";
  }
```
2. **closeSnack** - (required) function to close the alert
3. **state** - (required) state of the alert
```
state: {
    open: boolean;
    type: "success" | "error";
    message: string;
  }
```

### Usage

```jsx
import { Alert } from 'react-components'

const App = () => {
    const [state, setState] = useState({
        open: false,
        type: "success",
        message: "This is a success alert"
    })
    const closeSnack = () => {
        setState({
            ...state,
            open: false
        })
    }
    return (
        <Alert
            state={state}
            closeSnack={closeSnack}
        />
    )
}
```