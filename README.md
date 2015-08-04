# phpgh
git hooks for PHP

## Install
### per project
```git require --dev drx777/phpgh```
### globally
no need to modify the project's composer.json and disturbing your collegues
```git require global drx777/phpgh```

## Usage
add a call to the hooks script to your .git/hooks/pre-commit:

### per project
If installed for the project (registered in your project's composer.json), seee above section Install
```./vendor/bin/phpgh phpcs phplint phpunit```
### globally
```~/.composer/vendor/bin/phpgh phplint phpcs phpunit```

### available hooks

* phpcs
* phplint
* phpunit

## References
Using portions from <https://gist.github.com/cjsaylor/10503398>

## License

The MIT License (MIT)

Copyright (c) 2015 David Rekowski <david@rekowski.info>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
