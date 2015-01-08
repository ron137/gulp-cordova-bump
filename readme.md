> Bump your Semver in cordova projects

## Install

```sh
$ npm install --save-dev gulp-cordova-bump
```

## Add the following to your gulpfile

```js
var bump = require('gulp-cordova-bump');

gulp.task("bump", function(params)
{
    if (gulp.env.patch) {
        bump('patch');
    } elseif (gulp.env.minor) {
        bump('minor');
    } elseif (gulp.env.major) {
        bump('major');
    }
}
```
## Usage
```sh
$ gulp bump --patch
$ gulp bump --minor
$ gulp bump --major
```


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)