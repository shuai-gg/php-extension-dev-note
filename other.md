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


# php-config
php-config 是一个简单的命令行脚本用于获取所安装的 PHP 配置的信息。

在编译扩展时，如果安装有多个 PHP 版本，可以在配置时用 --with-php-config 选项来指定使用哪一个版本编译，该选项指定了相对应的 php-config 脚本的路径。

php-config 脚本在命令行所能使用的选项可以通过 -h 选项来显示

**命令行选项**

|  			选项   | 说明  |
|  ----  			| ----  |
| --prefix  		| PHP 所安装的路径前缀，例如 /usr/local |
| --includes  	| 列出用 -I 选项包含的所有文件 |
| --ldflags		|PHP 编译时所使用的 LD 标志|
| --libs	PHP		|编译时所附加的库|
| --extension-dir|扩展库的默认路径|
| --include-dir	|头文件的默认路径前缀|
| --php-binary 	|PHP CLI 或者 CGI 可执行文件的完整路径|
| --php-sapis		|列出所有可用的 SAPI 模块|
| --configure-options|重现当前 PHP 在编译时的配置选项|
| --version		|PHP 版本号|
| --vernum		|PHP 版本号，以整数表示|


#make

**Make工具常见的目标**：

make all：编译程序、库、文档等（等同于make）

make install：安装已经编译好的程序。复制文件树中到文件到指定的位置

make unistall：卸载已经安装的程序。

make clean：删除由make命令产生的文件

make distclean：删除由./configure产生的文件

make check：测试刚刚编译的软件（某些程序可能不支持）

make installcheck：检查安装的库和程序（某些程序可能不支持）

make dist：重新打包成packname-version.tar.gz





