# `stratic-date-in-path`

[Gulp][1] plugin to take a Vinyl file with [Stratic][2] post information (for example, something that's been parsed with [`stratic-parse-header`][3]) and make the file path include the year and month, as is typical in blog engines.

## Installation

    npm install stratic-date-in-path

## Usage

`gulpfile.js`:

```js
var gulp = require('gulp')
var straticParseHeader = require('stratic-parse-header');
var straticDateInPath = require('stratic-date-in-path');

gulp.task('parse', function() {
    gulp.src('*.md')
        .pipe(straticParseHeader())
        .pipe(straticDateInPath());
});
```

Each file's path now contains the year and month. For example, `hello-world.md` might be changed to `/2016/01/hello-world.md`.

## License

LGPL 3.0+

## Author

Alex Jordan <alex@strugee.net>

 [1]: http://gulpjs.com/
 [2]: https://github.com/strugee/generator-stratic
 [3]: https://npmjs.com/package/stratic-parse-header
