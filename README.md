# testcafe-reporter-spec-errors-summary
[![Build Status](https://travis-ci.org/dskochubey/testcafe-reporter-spec-errors-summary.svg)](https://travis-ci.org/dskochubey/testcafe-reporter-spec-errors-summary)

This is the **spec-errors-summary** reporter plugin for [TestCafe](http://devexpress.github.io/testcafe). The main difference from built-in **spec** report is this one shows summary of all error next to test execution result.

<p align="center">
    <img src="https://raw.github.com/dskochubey/testcafe-reporter-spec-errors-summary/master/media/preview.png" alt="preview" />
</p>

## Install 

```
npm install testcafe-reporter-spec-errors-summary
```

## Usage

When you run tests from the command line, specify the reporter name by using the `--reporter` option:

```
testcafe chrome 'path/to/test/file.js' --reporter spec-errors-summary
```


When you use API, pass the reporter name to the `reporter()` method:

```js
testCafe
    .createRunner()
    .src('path/to/test/file.js')
    .browsers('chrome')
    .reporter('spec-errors-summary') // <-
    .run();
```

## Author
Dmitry Kochubey 
