# AuthenticatedRoutes
> Routing component made with react-router-dom


### Props
1. authenticated - (required) Boolean value to check if user is authenticated or not
2. privateRoutes - (not required) ```RouteTypes[]``` Array of private routes
3. publicRoutes - (not required) ```RouteTypes[]``` Array of public routes
4. generalRoutes - (not required) ```RouteTypes[]``` Array of general routes
5. loading - (not required) set it to true, if you want to show loading animation
6. loadingComponent - (not required) if not set then default animation will show, set it to show your own loading component

### RouteTypes
> same as react-router-dom RouteProps
1. path - (required) path of the route
2. element - (required) component to render
3. children - (not required) children routes


### Usage
```tsx
import { AuthenticatedRoutes } from 'react-components';

const App = () => {
    return (
        <AuthenticatedRoutes
            authenticated={true}
            privateRoutes={[
                {
                    path: '/dashboard',
                    component: Dashboard,
                },
            ]}
            publicRoutes={[
                {
                    path: '/login',
                    component: Login,
                },
            ]}
            generalRoutes={[
                {
                    path: '/',
                    component: Home,
                },
            ]}
        />
    );
};
```