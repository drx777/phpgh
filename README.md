[![Latest Stable Version](https://poser.pugx.org/drx777/phpgh/v/stable)](https://packagist.org/packages/drx777/phpgh) [![Total Downloads](https://poser.pugx.org/drx777/phpgh/downloads)](https://packagist.org/packages/drx777/phpgh) [![Latest Unstable Version](https://poser.pugx.org/drx777/phpgh/v/unstable)](https://packagist.org/packages/drx777/phpgh) [![License](https://poser.pugx.org/drx777/phpgh/license)](https://packagist.org/packages/drx777/phpgh)

# phpgh
git hooks for PHP

## Purpose
This package wants to provide a simple way of adding git hooks to a project, even a number of projects without having to mess with multiple project's .git/hooks/* scripts repeatedly. Install via composer and add a line to the hook script. Done.

It can be used to kickstart your own centralized git hooks or as a basis for a company policy git hook collection.

## Status
This is an early proof-of-concept version. Any constructive feedback and suggestions are welcome.

## Install
### globally (recommended)
no need to modify the project's composer.json and disturbing your collegues

```$ composer require global drx777/phpgh```

add a call to the hooks script to your git project's .git/hooks/pre-commit (make sure the script is executable):

```~/.composer/vendor/bin/phpgh phplint phpcs phpunit```

### per project
```$ composer require --dev drx777/phpgh```

add a call to the hooks script to your git project's .git/hooks/pre-commit (make sure the script is executable):

```./vendor/bin/phpgh phpcs phplint phpunit```

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
