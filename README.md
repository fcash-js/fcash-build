# fcash-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install fcash-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var fcashBaseTasks = require('fcash-build');

fcashBaseTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var fcashBaseTasks = require('fcash-build');
fcashBaseTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/fcash-js/fcash-base) on the main fcash-base repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/fcash-js/fcash-base/blob/master/LICENSE).

Copyright 2015 Fcash, Inc. Fcash is a trademark maintained by Fcash, Inc.

