# Select
> Select component made with [@mui/material/Select](https://mui.com/material-ui/react-select/)
### Props
1. **options** - (required) Array of options for the select
2. **label** - (required) Label for the select
3. **control** - (required) Control from react-hook-form
4. **name** - (required) Name of the select
5. **sx** - (not required) sx props from @mui/material
6. **fullWidth** - (not required) if true then select will be full width

### Usage
```tsx
import { Select } from 'react-components';
import { Control } from 'react-hook-form';

const App = () => {
    const { control } = useForm();
    return (
        <Select
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