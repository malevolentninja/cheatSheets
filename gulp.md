# Gulp notes

| Keyword | Explanation |
|--------|:-------------------------------:|
| Basic Format | ```gulp.task('task-name', function() { // Stuff here });``` |
| Run a task in gulp | gulp task-name |
| task example format | ```gulp.task('task-name', function () { return gulp.src('source-files') // Get source files with gulp.src .pipe(aGulpPlugin()) // Sends it through a gulp plugin .pipe(gulp.dest('destination')) // Outputs the file in the destination folder })```|
| install gulp plugin | gulp-pluginName|
| gulp-watch | ```gulp.watch('files-to-watch', ['tasks', 'to', 'run']);```  |
| browser-sync | synchronises the browser, can link into gulp-watch task to run at the same time as other plugins |
| gulp-concatenate | Joins scripts together but doesn't really work if the scripts are located in multiple different directories |
| gulp-useref | concatenates any number of css and js files into a single file. It looks for a comment starting with ``` <!--build: <type> <path> --> script and link tags <!--endbuild -->``` Automatically changes all the scripts within ```<!--build:``` and ```<!--endbuild-->``` into one single JavaScript file that points to whereever you directed it to. |
| gulp-uglify |  minifies javascript files |
| gulp-if | ensures we only attempt to minify javascript files.  |
| gulp-cssnano | minify concatenated css files |
| gulp-imagein | helps optimise images |
| gulp-cache |  part of the optimisation process, caches the images which went through the imagemin process. |
| del | npm cleans the app. Any files which are no longer in use can be deleted. |
| run sequence | ensure the cleans are completed before the rest of the tasks are undertaken. The first task will run. When one is complete, two will automatically start. ```gulp.task('task-name', function(callback) { runSequence('task-one', 'task-two', 'task-three', callback); }); // can also be placed in an array form:  gulp.task('task-name', function(callback) { runSequence('task-one', ['tasks','two','run','in','parallel'], 'task-three', callback); });``` |
|  default | creating a task named default mean it can be run by simply naming gulp - saving on keystrokes! |
