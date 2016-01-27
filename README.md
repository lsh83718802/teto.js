[![Build Status](https://img.shields.io/travis/crossjs/teto.js.svg?style=flat-square)](https://travis-ci.org/crossjs/teto.js)
![David](http://img.shields.io/david/crossjs/teto.js.svg?style=flat-square)
![David](http://img.shields.io/david/dev/crossjs/teto.js.svg?style=flat-square)
![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat-square)

## Installation

```
$ npm install
```

## Running Dev Server

```
$ npm start
```

## Tips

- RHL@1.x 会导致 @autobind 不可用，所以采用 2.x
- 除了 decorator，还可以使用操作符 `::` 来实现 autobind，参见：http://babeljs.io/blog/2015/05/14/function-bind/
- 开发时不应使用 extract-text-webpack-plugin，因为它让 CSS 无法热替换
- Object.assign 与 Array.slice 都不是深拷贝
- 组件的 key 参数使用时应避免使用索引值，而应该使用 id 等唯一值
- 标签的嵌套要注意符合 W3C 规范，比如 button 不能嵌套 button、table 需要 tbody
- 所有路由在 `routes` 目录下，为了实现异步加载，对应的 component 以 `.async.js(x)` 结尾

# node-sass

如果收到提示：`ERROR in The `libsass` binding was not found`，则可以尝试：

```
$ npm rebuild node-sass
```

[![](teto.png)](http://seiga.nicovideo.jp/seiga/im2044734)
