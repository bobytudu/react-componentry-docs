# Input
> made with @mui/material/TextField, also inherits all the props of the [@mui/material/TextField](https://mui.com/material-ui/react-text-field/) element.
### Props
1. **label** - (required) Label for the input
2. **name** - (required) Name of the input
3. **type** - (not required) Type of the input
4. **rows** - (not required) required if multiline is true;
5. **multiline** - (not required) if true then input will be multiline
6. **disabled** - (not required) if true then input will be disabled
7. **placeholder** - (not required) placeholder for the input

### Usage
```jsx
import { Input } from 'react-components'
import { Control } from 'react-hook-form'

const App = () => {
    const { control } = useForm()
    return (
        <Input
            control={control}
            name="name"
            label="Name"
            type="text"
            placeholder="Enter your name"
        />
    )
}
```