# 微光招新第一题

## 1.hello.c的创建及运行

```
#include<stdio.h>
int main()
{
    printf("hello,world!");
    return 0;
}
//hurundong
```

此为我所编写的代码

## 2.高级计算机语言与低级计算机语言，各有什么优劣，你更喜欢哪一类计算机语言？

1. 就我所知C++、Java、Python、C#等都是高级语言，相对于低级语言来说，高级语言采用易于识别和记忆的字符来作为关键字，也更接近人类的思维方式，编写容易读写性好，开发效率更高，但是我觉得它的执行效率并不如低级语言，使用高级语言编写的程序运行时，需要先将其翻译成低纸语言计算机才能运行它。
2. 泛指机器语言和汇编语言，其中，机器语言是计算机最原始的语言，由0和1的代码构成，计算机在工作的时候只认识机器语言，即0和1的代码；汇编语言，它用人类容易记忆的语言和符号来表示一组0和1的代码。他执行速度快，但代码编写难度较大，可读性较差。

3. 我个人更喜欢高级语言因为它易懂更容易被人类所接受。

## 3.尝试解读hello.c中每一行的内容。

1. 第一行`#include<stdio.h>`此为头文件，如果没有这个编译器都不知道`printf`是个什么东东，我认为头文件就是一个准备好的大仓库，你可以取用你需要的来增加代码效率。
2. 第二行`int main()` 是一个函数，它在C语言程序中扮演着至关重要的角色，它是程序的入口，即执行开始的地方。
3. 第三行{}该括号可以使其中的代码具有一定的独立性，使其中定义的变量无法被括号外访问
4. 第四行`printf`是输出函数，可以用于输出信息
5. 第五行`return 0`我觉得它是返回0这个值，代表着函数的终止运行

## 4.删去该程序的哪一行不会影响运行结果？

删去`return 0`不会影响结果。

## 5.int类型是计算机存储什么元素的方式？为什么main函数要使用int进行声明/定义？

1. int是整数类型。
2. ，而第二个问题我认为是:  一般情况下，返回 0 表示程序正常结束  ,  使用 int 类型可以方便地地接收和处理其他函数的返回值，以便操作系统或其他程序能够了解程序的执行结果。

## 6.请调整上述程序的内容，使其输出内容改为Hello gilmmer!并附上运行截图

![hello,world!与hello,gilmmer!在vs code上的运行截图](C:\Users\91496\Desktop\招新作业\微光第一题\第一题程序运行截图\hello,world!与hello,gilmmer!在vs code上的运行截图.png)

此为在vs code上的运行结果（hello,world!与hello,gilmmer!)

## 7.修改小明的代码

```
#include <stdio.h>

int main() {
    int code;
    int i;
	printf("Show me your code,please.");
    scanf("%d",&code);
    while(i!=-1){
        if(code >= 100000 && code <= 999999){
        printf("I am super hacker!");
        i = -1;
    }else printf("Fake code!");
          scanf("%d",&code);
    }
    return 0;
}
```

### 8.课后题

```
#include <stdio.h>

int main()
{  
    int a,b;
    int t;
    scanf("%d %d",&a,&b);
    
    while(b!=0){
    	t=a%b;
    	a=b;
    	b=t;	
	}
	printf("%d",a);
    return 0; 
}
```

注：以上所有答案均为在翁恺老师视频，知乎，博客，bilibili，csapp所查阅及思考得出,未使用gpt及任何AI
