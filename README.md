# mt-spinner
> spinner.

## Install
```shell
npm i kb-spinner -S
```

## Required
```shell
npm i babel-plugin-component -D
```

## Usage
import all spinner
```javascript
import Vue from 'vue';
import Spinner from 'mt-spinner';

Vue.use(Spinner);
```

```html
<mt-spinner></mt-spinner>
```

import one spinner
```javascript
import Vue from 'vue';
import { DoubleBounce } from 'mt-spinner';

Vue.component(DoubleBounce.name, DoubleBounce);
```

```html
<double-bounce></double-bounce>
```

.babelrc
```json
{
  "plugins": [
    "xxx",
    ["component", [
        {
          "libraryName": "mt-spinner",
          "style": true
        }
      ]
    ]
  ]
}
```

## Spinner
- snake
- double-bounce
- triple-bounce
- fading-circle

## API

### color
- type: String

### size
- type: Number

### type
- type: String|Number

```html
<mt-spinner :type="0"></mt-spinner>
<mt-spinner type="snake"></mt-spinner>

<mt-spinner :type="1"></mt-spinner>
<mt-spinner type="double-bounce"></mt-spinner>

<mt-spinner :type="2"></mt-spinner>
<mt-spinner type="triple-bounce"></mt-spinner>

<mt-spinner :type="3"></mt-spinner>
<mt-spinner type="fading-circle"></mt-spinner>
```

## Development

```shell
make dev
```

## Production
```
make dist
```

## License
MIT
