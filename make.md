**Make工具常见的目标**：

make all：编译程序、库、文档等（等同于make）

make install：安装已经编译好的程序。复制文件树中到文件到指定的位置

make unistall：卸载已经安装的程序。

make clean：删除由make命令产生的文件

make distclean：删除由./configure产生的文件

make check：测试刚刚编译的软件（某些程序可能不支持）

make installcheck：检查安装的库和程序（某些程序可能不支持）

make dist：重新打包成packname-version.tar.gz