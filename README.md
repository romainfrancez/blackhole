blackhole [![Build Status](https://travis-ci.org/romainfrancez/blackhole.png?branch=master)](https://travis-ci.org/romainfrancez/blackhole) [![Code Climate](https://codeclimate.com/github/romainfrancez/blackhole.png)](https://codeclimate.com/github/romainfrancez/blackhole)
=========

An empty function to discard results.

Example
------
```javascript
var blackhole = require('blackhole');

function aFunction (someArgs, callback) {
  callback = callback || blackhole;

  callback(someErr, someValue); // No need for a check on callback anymore
}
```