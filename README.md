until the livereload issue /pull request is handled you need to hack the reloadPage in livereload

vim node_modules/ember-cli/node_modules/tiny-lr/node_modules/livereload-js/dist/livereload.js

```
    return this.reloadPage(path);
```

It should look like the above (we need to hack this so we can get a hook client side)

# Ember-cli-hot-loader

This README outlines the details of collaborating on this Ember addon.

## Installation

* `git clone` this repository
* `npm install`
* `bower install`

## Running

* `ember serve`
* Visit your app at http://localhost:4200.

## Running Tests

* `npm test` (Runs `ember try:testall` to test your addon against multiple Ember versions)
* `ember test`
* `ember test --server`

## Building

* `ember build`

For more information on using ember-cli, visit [http://ember-cli.com/](http://ember-cli.com/).
