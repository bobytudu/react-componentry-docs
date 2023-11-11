# DatePicker
> Customized version of [@mui/x-date-pickers/DatePicker](https://mui.com/x/react-date-pickers/date-picker/)
### Props
1. **label** - (required) Label for the DatePicker  
2. **name** - (required) Name of the DatePicker
3. **control** - (required) Control from react-hook-form
4. **fullWidth** - (not required) if true then DatePicker will be full width

## Usage

```jsx
import { DatePicker } from 'react-components'
import { Control } from 'react-hook-form'

const App = () => {
    const { control } = useForm()
    return (
        <DatePicker
            control={control}
            name="name"
            label="Name"
        />
    )
}
```