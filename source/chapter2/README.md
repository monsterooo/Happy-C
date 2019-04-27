# 第二章总结

## 基础知识

* printf 格式化字符串输出
* scanf 格式化字符串输入
* #define name value 用来定义一个常量/宏定义(macro definition)
* c 标识符区分大小写，大家都遵守标识符使用小写宏定义使用大写。单词间的分割使用_(下划线分割)
* printf  (  "Height: %d\n"  ,  height  )  ;
    1     2          3       4    5     6  7
  每个数字都是一个记号(token)，其中记号1和5都是标识符，记号3是字符串字面量。记号2、4、6、7则是标点符号

## 关键字

auto enum restrict(c99) unsigned break extern return void case float short volatile char for signed while const goto sizeof _Bool(c99) continue if static _Complex(c99) default inline(c99) struct _Imaginary(c99) do int switch double long typedef else register union

## gcc

常用选项
-Wall     是编译器在检测到可能的错误时生成警告信息。
-pedantic 根据C标准的要求生成警告消息。这样避免在程序中使用非标准特性
-ansi     禁用GCC的非标准C特性，并启用一些不太常用的标准特性
-std=c89  指定使用哪个版本的编译器来检查程序

使用：
gcc -O -Wall -pedantic -ansi -std=c99 -o pun pun.c