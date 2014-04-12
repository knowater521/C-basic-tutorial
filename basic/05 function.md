<a href="http://www.lellansin.com/wp-content/uploads/2012/10/QQ截图20121025184614.jpg"><img class="alignnone size-full wp-image-87" title="函数的基本概念" src="http://www.lellansin.com/wp-content/uploads/2012/10/QQ截图20121025184614.jpg" alt="" width="874" height="639" /></a>

[code lang="c"]
// 初中
y = 3x + 2

// 高中
f(x) = 3x + 2

// c语言
int f(int x)
{
    return x * 3 + 2;
}
[/code]

<h1>C语言中的函数</h1>

1.函数名
2.参数
3.返回值

[code lang="c"]
#include <stdio.h>

/*
    sum函数名 返回值为int
    int a, int b 为sum的参数及其类型
    返回值为 ( a + b ) 这个表达式的值
*/
int sum(int a, int b)
{
    return a + b;
}

main()
{
    int i, j;
    printf("请输入两个数：\n");
    scanf("%d%d", &i, &j);
    printf("%d\n", sum(i, j)); // sum(参数,参数)的形式调用,返回两数之和
}
[/code]

<h2>函数的作用域</h2>

[code lang="c"]
#include <stdio.h>

void swap(int i, int j)
{
    int temp;
    temp = i; i = j; j = temp;
    printf("x=%d, y=%d", x, y);
}

main()
{
    int i = 30, j = 75;
    swap(i, j);
    printf("i=%d, j=%d\n", i, j),
}
[/code]

main()中的 i, j 与 swap() 中的 i,j 不是相同的变量
两个函数,是两个不同的内存块.两个变量名称相同,但不在同一个内存上
所以,如果其中某个变量有改变与另一个函数中的变量无关

<h1><a title="链向 c语言入门教程 第6讲 编译预处理命令 的固定链接" href="http://www.lellansin.com/?p=89" rel="bookmark">c语言入门教程 第6讲 编译预处理命令</a></h1>