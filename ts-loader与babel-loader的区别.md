# 相同点
  将js、jsx、ts、tsx 或者 ES6＋的代码 编译成 兼容性高的原生js
# 区别
1. ts-loader：`编译`＋`语法检查`
   > 编译过程中如果出现ts语法错误，在terminal中会有错误提示
   babel-loader：`编译`＋`无语法检查`
   > 编译过程中不管有没有ts语法错误

2. ts-loader：`无polyfill` 功能
   babel-loader：通过预设或者插件可以添加polyfill，例如Promise、Proxy、Symbol等等

# Why use babel-loader with ts-loader?
https://stackoverflow.com/questions/49624202/why-use-babel-loader-with-ts-loader

如果没有使用 Babel，首选 TypeScript 自带编译器（配合 ts-loader 使用）
如果项目中有 Babel，安装 @babel/preset-typescript，配合 tsc 做类型检查。
两种编译器不要混用。