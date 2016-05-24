# kb-spinner
> spinner.

## Install
```shell
npm i kb-spinner -S
```

## Usage
import all spinner
```javascript
import Vue from 'vue';
import Spinner from 'kb-spinner';
import 'kb-spinner/all/style.css'

Vue.use(Spinner);
```

import one spinner
```javascript
import Vue from 'vue';
import DoubleBounce from 'kb-spinner/dobule-bounce';
import 'kb-spinner/dobule-bounce/style.css';

Vue.component(DoubleBounce.name, DoubleBounce);
```

## API

### color
- type: String

### size
- type: Number

### type
- type: String|Number

```javascript
<kb-spinner :type="0"></kb-spinner>
<kb-spinner type="snake"></kb-spinner>

<kb-spinner :type="1"></kb-spinner>
<kb-spinner type="double-bounce"></kb-spinner>

<kb-spinner :type="2"></kb-spinner>
<kb-spinner type="three-bounce"></kb-spinner>

<kb-spinner :type="3"></kb-spinner>
<kb-spinner type="fading-circle"></kb-spinner>
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