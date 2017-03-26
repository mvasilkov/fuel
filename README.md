# What's this?

The FuelDOM is React compatible virtual-dom implementation.

* File size is samller than Reactjs **8kb(raw 16kb)**
* Change vdom patch function as using requestAnimationFrame and requestIdleCallback.
* Compatible with jsx.

## Installation

```shell
npm install fueldom --save
```

## Usage

### Simple rendering

```javascript
import {
  Fuel,
  React,
  FuelDOM
} from 'fueldom';

class Component extends Fuel.FuelComponent {
  render() {
    return (
      <div>
        <span>Hello World</span>
      </div>
    )
  }
}

FuelDOM.render(<Component/>, document.getElementById('app'));
```

## Future

### WE WON't DO

* 100% compatiblity with React.
* React fiber.

### WE WILL DO

* Improve code size to make it more samll.
* Improve vdom patch method to make it more fast.
* Original functionarity or api.

## Contribute

Fork!

```
npm install
npm run test
npm run minify
```