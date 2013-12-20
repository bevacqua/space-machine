# space-machine

> Split a string by spaces. Use .spawn like an .exec!

# Install

```shell
npm i -S space-machine
```

# Usage

```js
var spawn = require('child_process').spawn;
var machine = require('space-machine');
var command = 'node app --foo "bar baz"';

var args = machine(command);
// <- ['node', 'app', '--foo', '"bar baz"']

var program = args.shift();

spawn(program, args);
```

# License

MIT
