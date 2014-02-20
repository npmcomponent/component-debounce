*This repository is a mirror of the [component](http://component.io) module [component/debounce](http://github.com/component/debounce). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/component-debounce`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# debounce

  Useful for implementing behavior that should only happen after a repeated action has completed.

## Installation

    $ component install component/debounce

  Or in node:

    $ npm install debounce

## Example

```js
var debounce = require('debounce');
window.onresize = debounce(resize, 200);

function resize(e) {
  console.log('height', window.innerHeight);
  console.log('width', window.innerWidth);
}
```

## API

### debounce(fn, wait, [ immediate || false ])

  Creates and returns a new debounced version of the passed function that will postpone its execution until after wait milliseconds have elapsed since the last time it was invoked.

  Pass `true` for the `immediate` parameter to cause debounce to trigger the function on the leading edge instead of the trailing edge of the wait interval. Useful in circumstances like preventing accidental double-clicks on a "submit" button from firing a second time.

## License

  MIT
