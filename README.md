# `stratic-date-in-path`

[Gulp][1] plugin to take a Vinyl file with [Stratic][2] post information (for example, something that's had YAML frontmatter parsed with [`gulp-gray-matter`][3]) and make the file path include the year and month, as is typical in blog engines.

## Installation

    npm install stratic-date-in-path

## Usage

`gulpfile.js`:

```js
var gulp = require('gulp')
var frontMatter = require('gulp-gray-matter');
var straticDateInPath = require('stratic-date-in-path');

gulp.task('posts', function() {
    gulp.src('*.md')
        .pipe(frontMatter())
        .pipe(straticDateInPath());
});
```

Each file's path now contains the year and month. For example, `hello-world.md` might be changed to `/2016/01/hello-world.md`.

## Code of Conduct

Please note that StraticJS is developed under the [Contributor Covenant][4] Code of Conduct. Project contributors are expected to respect these terms.

For the full Code of Conduct, see [CODE_OF_CONDUCT.md][5]. Violations may be reported to <alex@strugee.net>.

## License

LGPL 3.0+

## Author

Alex Jordan <alex@strugee.net>

 [1]: http://gulpjs.com/
 [2]: https://github.com/strugee/generator-stratic
 [3]: https://npmjs.com/package/gulp-gray-matter
 [4]: http://contributor-covenant.org/
 [5]: https://github.com/straticjs/stratic-date-in-path/blob/master/CODE_OF_CONDUCT.md
