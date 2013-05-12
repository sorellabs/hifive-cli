# brofist-cli

An convenient command line runner for [Brofist][].

[Brofist]: http://github.com/brofistjs/brofist


## Usage

The simplest form is to just give `brofist` a directory with your specs, and
we'll execute all files under that directory.

    $ brofist tests/specs
    
You can also give one or more spec modules directly, in which case we'll only
run those files:

    $ brofist tests/specs/foo.js tests/specs/bar.js
    
You can change the reporter being used with the `--reporter` option, check 'em
`brofist list` to get a list of available reporters.


## Brofist(1)


    brofist --- runner for Brofist tests

    Usage:
      brofist [options] <files...>
      brofist list
      brofist -h, --help
      brofist --version

    Options:
      -r, --reporter <module>   Reporter module to use. [default: 'brofist-reporter']
      -f, --filter <regexp>     Only runs tests that match the regexp.
      -t, --timeout <ms>        Timeout for asynchronous tests, in milliseconds.
      -s, --slow <ms>           Slow threshold, in milliseconds.
      -h, --help                Displays usage help and exits.
      --version                 Displays version number and exits.

      
      
## Installing

Grab it from NPM:

    $ npm install -g brofist-cli
    

## Licence

MIT/X11. Do whatever you want.