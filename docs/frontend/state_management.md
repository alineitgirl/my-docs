# State Management in React

The frontend uses a combination of **React Context** and **React Query**.

## Local State

- Use component-level `useState` for UI interactions, form values, modal open/close states
- Keep state as close as possible to where it’s used

## Global State

- **React Context** is used for:
  - Theme (dark/light)
  - Authentication state
  - User settings

```javascript
// Example: AuthContext
const AuthContext = createContext();

export const AuthProvider = ({ children }) => {
  const [user, setUser] = useState(null);

  return (
    <AuthContext.Provider value={{ user, setUser }}>
      {children}
    </AuthContext.Provider>
  );
};
```

## Server State
 
- **React Query** handles server data, caching, and background updates

- Example: Fetching tasks

```javascript
const { data: tasks, isLoading } = useQuery('tasks', fetchTasks);
```

## Optimization Tips

- Use **useMemo** and **useCallback** to prevent unnecessary re-renders
- Split large components into smaller ones
- Keep API requests centralized in hooks or services


