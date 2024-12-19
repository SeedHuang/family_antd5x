# FASelect

This is an example component.

```jsx
import { FASelect } from 'family_antd5x';
import { useState, useCallback} from 'react';

const options=[
  { value: 'jack', label: 'Jack' },
  { value: 'lucy', label: 'Lucy' },
  { value: 'Yiminghe', label: 'yiminghe' },
];

export default () => {
  const [value, setValue] = useState('jack');
  const onSelectChangeHandler = useCallback((value) => {
    setValue(value);
  
  }, [setValue])
  return <FASelect value={value} options={options} onChange={onSelectChangeHandler}/>
}
```
