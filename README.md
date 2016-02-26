# getopt

## About

This package provides a module for analyzing a list of command-line
arguments. It uses a command-line syntax similar to the GNU ``getopt_long``
function. The package also provides an automated test suite which
uses the ptester library from http://b9.com/files/ptester/

## Running Tests

getopt comes with unit tests. In order to run them, you'll need to do the following first:

```cl
* (ql:quickload "ptester")
...
("ptester")
* (asdf::load "getopt.asd")
T
* (asdf:load-system "getopt-tests")
...
T
```

You can then run them with the following:

```cl
* (getopt-tests::do-tests)
Begin GETOPT test

**********************************
End GETOPT test
Errors detected in this test: 0
Successes this test:26
T
```
