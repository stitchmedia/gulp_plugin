## gulp-utf8-convert

a plugin for gulp.js to convert file encoding to utf8

## Installation

```bash
npm install gulp-utf8-convert
```

## Usage

```js
var gulp = require('gulp');
var utf8Convert = require('gulp-utf8-convert');

gulp.task('convert',function() {
    gulp.src("./test.txt")
        .pipe(utf8Convert({
            encNotMatchHandle:function (file) {
                //notify
            }
        }))
        .pipe(gulp.dest('./'));
});
```
