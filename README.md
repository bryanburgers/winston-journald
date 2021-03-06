# winston

A journald transport for [winston][0].

## Motivation
`tldr;?`: To break the [winston][0] codebase into small modules that work
together.

The [winston][0] codebase has been growing significantly with contributions and
other logging transports. This is **awesome**. However, taking a ton of
additional dependencies just to do something simple like logging to the Console
and a File is overkill.

## Usage
``` js
  var winston = require('winston');

  /**
   * Requiring `winston-journald` will expose
   * `winston.transports.journald`
   */
  require('winston-journald').Journald;

  winston.add(winston.transports.Journald, options);
```


## Installation

``` bash
  $ npm install winston
  $ npm install winston-journald
```

#### Author: [Romain CATOIO](http://rocat.fr)

[0]: https://github.com/flatiron/winston
