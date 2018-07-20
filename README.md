# TwigTools
Twigtools is a PyroCMS plugin, providing useful tools for development and debugging with twig. 

Initially this provides the following functions inside twig templates:

- `dd` Dumps an item and kills the rest of the page.
- `debug` Dumps an item and continues execution
- `debug` Debugs an item to [Debugbar](https://github.com/barryvdh/laravel-debugbar) under the Messages tab

### Installing

You can install this plugin into your existing PyroCMS 3.x installation by requiring it inside your composer file:

```
"require-dev": {
    "evoluted/twigtools-plugin": "~1.0",`
}
```

Or by running the command line composer install command:

`composer require evoluted/twigtools-plugin`

Once installed you will not have to perform any additional actions to start using this plugin.

### Usage

#### dd
`dd(yourVariable)`

Uses [Laravels dump method](https://laravel.com/docs/5.6/helpers#method-dump), and stops execution.

#### dump
`dump(yourVariable)`

Uses [Laravels dump method](https://laravel.com/docs/5.6/helpers#method-dump), but continues rendering the rest of the page.

#### debug
`debug(yourVariable)`

Debugs a variable to [Laravel Debugbar](https://github.com/barryvdh/laravel-debugbar) (if it is installed)

## Future Ideas

- Manipulation of objects and arrays (E.g resorting, inserting within arrays, etc)
- Debug to log files from within twig

## Release History
* 1.0.0
    * Initial release, containing `dd()`, `debug()`, `debug()`

## Contributing

1. Fork it (<https://github.com/EvolutedNewMedia/pyrotwigtools/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request