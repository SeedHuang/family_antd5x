# FAInput

This is an example component.

```jsx
import { FAInput } from 'family_antd5x';
import { useState, useCallback} from 'react';

export default () => {
  const [value, setValue] = useState('This is a test value');
  const onInputChangeHandler = useCallback((event) => {
    setValue(event.target.value);
  }, [setValue])
  return <FAInput value={value} onChange={onInputChangeHandler}/>
}
```
