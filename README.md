# fis sass parser

基于https://github.com/lwdgit/fis-parser-sass2修改。

可以通过引入文件的方式引入sass变量。

```javascript
//fis3-conf.js
fis.match('**/*.scss', {
    rExt: '.css',
    parser: fis.plugin('sass2', {
        'import': 'static/css/variables.scss'
    })
});
