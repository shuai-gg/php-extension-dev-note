# configure

### configure的配置项

**编译php**

- --prefix
设置php安装目录
- --enable-maintainer-mode
对偶然安装一下的情形启用此选项，使得不检查编译规则和依赖关系。

- --with-config-file-path=PATH
设置 php.ini 的搜索路径。默认为 PREFIX/lib。

- --enable-safe-mode
默认启用安全模式。

- --enable-zend-multibyte
在词法与语法分析时允许多字节编码被执行。如果在编译PHP时使用了这个选项，就能够在 declare 结构中使用 encoding指令。



**编译扩展**

- --with-php-config
指定扩展编译安装的php版本


Tag:
为什么有的扩展的开启方式是 --enable-extname的形式，有的则是--with-extname的形式呢？
enable多代表不依赖外部库便可以直接编译，而with大多需要依赖于第三方的lib