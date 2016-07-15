ginkgo
# server 端不需要打包，相对而言server端环境可控，无需处理。倒是可以压缩

# client 端使用node风格的代码，需要打包，才能在各浏览器兼容

1/错误汇报机制，捕获错误，并提交到数据中心进行收录


# 命名规范
所有的链接url，文件名称，样式/id名称，key值，cookie名称,以小写加分隔符命名 hello-world
所有的类首字母大写骆峰法命名 Hello/HelloWord
所有的function以及类方法以首字母小写骆峰法命名 helloWorld
所有的日志以[error|info|debug]-[module]-yyyyMMddhhmm.log命名 error-app-20160713120703.log
所有的常量以全大写加_下划线分隔 SERVER_URL
变量名一律小写加下划线 hello_world
所有的字符串以双引号表示，所有的json对象属性名称使用双引号

包含
browserify（组织浏览器代码）
gulp（编译打包工具）
npm（模块安装工具）
bower（前端模块安装工具）
express（服务器）
react（前端组件）
react-with-style（前端组件样式mixed混合）
jquery（前端工具）
jquery-cookie（前端cookie操作）
jquery-validate（表单校验）
reset-css（初始样式清除）
animate-css（动画样式库）
request（服务端请求）
ejs（服务端模板）
log4js（日志记录）
xml2js（xml解析生成模块）
node-redis（服务器端缓存）
mysql（数据库链接工具）
nodemon（自动重启）
babel(es6代码降级兼容)
pm2（服务器守护进程）
uuid
gulp-replace
gulp-clean-css
gulp-uglify
gulp-htmlmin
gulp-json-minify
gulp-plumber
gulp-run-sequence
gulp-zip
gulp-ftp
gulp-size
gulp-notify

不包含
webpack(配置较难理解，如果未来脱离webpack，源码是否能很好运行)
grunt（配置繁琐）
forever（被nodemon/pm2取代）
browsersync（liveload看起来挺好，实际上启动慢，控制台多出一些无用信息，除非移动端远程调试需要，常规流程不使用它）
jade
typescript（babel ES6取代）
sass/less

未来包含功能
引入etcd
修复gulp-ftp上传问题


生成sitemap.xml规范http://www.sitemaps.org/protocol.html