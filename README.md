*This repository is a mirror of the [component](http://component.io) module [juliangruber/prefixed](http://github.com/juliangruber/prefixed). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/juliangruber-prefixed`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# prefixed

CSS vendor prefix helpers.

## Usage

```js
var prefixed = require('prefixed');

var el = document.querySelector('#el');

prefixed(el.style, 'transition', '1s');
// el now has
//   -moz-transition: 1s
//   -webkit-transition: 1s
//   -o-transition: 1s
//   -ms-transition: 1s
//   transition: 1s
```

## API

### prefixed(style, attribute, value)

Set `attribute` with all possible vendor prefixes on `style` to `value`.

### prefixed.get(style, attribute)

Get the value of `attribute` on `style`, taking vendor prefixes into account.

## Installation

With [npm](http://npmjs.org) do

```bash
$ npm install prefixed
```

Then bundle for the browser with
[browserify](https://github.com/substack/browserify).

## License

(MIT)

Copyright (c) 2013 Julian Gruber &lt;julian@juliangruber.com&gt;

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do
so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
