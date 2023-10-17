## Install

```bash
npm install --save react-kvn-funnel
```

> or

```bash
yarn add react-kvn-funnel
```

## Usage

```jsx

import { Funnel } from 'react-kvn-funnel';

```

##Simple example

```jsx

<Funnel
  height={252}
  colors={{
    graph: [ '#1890FF', '#BAE7FF' ],
    percent: 'red',
    label: 'yellow',
    value: 'orange'
  }}
  valueKey='quantity'
  width={800}
  data={data} />

```

##Render prop example

```jsx
const data = [
  {
      "label": "One Hundred",
      "quantity": 100
  },
  {
      "label": "Fifty",
      "quantity": 50
  },
  ...{}
]

  <Funnel
  labelKey='label'
  height={252}
  colors={{
    graph: [ '#1890FF', '#BAE7FF' ], // array or string : 'red' || '#666'
    percent: 'red',
    label: 'yellow',
    value: 'orange'
  }}
  valueKey='quantity' 
  width={800}
  displayPercent={true}
  data={data} />

```

| props          | Type            | Default Value          | Options      |
| -------------  |:--------------: | :--------------------: | :----------: |
| labelKey       | string          |                        |              |
| colors         | object          |                        |              |
| valueKey       | string          |                        |              |
| width          | number          | container width        |              |
| displayPercent | boolean         | false                  | false / true |
| data           | array           |                        |              |

## License

MIT © [kevin1193](https://github.com/kevin1193)