# 《PHP扩展开发学习笔记》目录
> 上一章: [《PHP扩展开发学习笔记》](<README.md>)
> 下一章: [配置编译环境](<1.md>)


1. [配置编译环境](1.md)
      1. [编译前的准备](1.1.md)
      2. [PHP编译前的config配置](1.2.md)
      3. [Unix/Linux平台下的编译](1.3.md)
      4. [在Win32平台上编译PHP](1.4.md)
      5. [小结](1.5.md)
2. [第一个扩展](5.md)
      1. [一个扩展的基本结构](2.1.md)
      2. [编译我们的扩展](5.2.md)
      3. [静态编译](5.3.md)
      4. [编写函数](5.4.md)
      5. [小结](5.5.md)
3. [函数的返回值](6.md)
      1. [一个特殊的参数：return_value](3.1.md)
      2. [引用与函数的执行结果](3.2.md)
      3. [小结](3.3.md)
4. [函数的参数](4.md)
      1. [zend_parse_parameters](4.1.md)
      2. [Arg Info 与类型绑定](4.2.md)
      3. [小结](4.3.md)
5. [Array与HashTable](5.md)
      1. [数组(C中的)与链表](5.1.md)
      2. [操作HashTable的API](5.2md)
      3. [在内核中操作PHP语言中数组](5.3.md)
      4. [小结](5.4.md)
6. [php生成uuid的扩展库](6.md)
      1. [关于UUID](6.1.md)
      2. [申明UUID导出函数](6.2.md)
      3. [声明Zend函数块](6.3.md)
      4. [实现UUID导出函数](6.4.md)