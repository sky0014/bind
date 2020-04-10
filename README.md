# sky-bind

Bind all your class methods with one line.

## Install

```bash
npm install sky-bind
```

## Usage

```js
import { bindAll } from "sky-bind";

class A {
  name = "A";

  constructor() {
    bindAll(this); // done, all your class methods have bind this already.
    // this.onclick = this.onclick.bind(this); // that's no need here
  }

  onclick() {
    console.log("hello", this.name); // this will always pointer to this A instance
  }
}
```
