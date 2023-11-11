# AutoComplete
>Customized AutoComplete component from [@mui/material/AutoComplete](https://mui.com/material-ui/react-autocomplete/)
### Props
1. **options** - (required) Array of options for the select
2. **label** - (required) Label for the select
3. **control** - (required) Control from react-hook-form
4. **name** - (required) Name of the select
5. **sx** - (not required) sx props from @mui/material
6. **fullWidth** - (not required) if true then select will be full width
7. **loading** - (not required) if true then loading will be shown
8. **multiple** - (not required) if true then select will be multiple
9. **disableCloseOnSelect** - (not required) if true then select will not close on select
10. **optionLabel** - (not required) if provided then it will be used to display the label of the option
11. **renderOption** - (not required) if provided then it will be used to render the option

### Usage
```tsx
import { AutoComplete } from 'react-components';
import { Control } from 'react-hook-form';

const App = () => {
    const { control } = useForm();
    return (
        <AutoComplete
            control={control}
            name="name"
            label="Name"
            options={[
                { value: '1', label: 'One' },
                { value: '2', label: 'Two' },
                { value: '3', label: 'Three' },
            ]}
        />
    );
};
```