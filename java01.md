#  ***java的学习路线***



![image-20200531194136272](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531194136272.png)

![image-20200531194158037](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531194158037.png)

![image-20200531194220917](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531194220917.png)

![image-20200531194258819](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531194258819.png)

![image-20200531194324274](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531194324274.png)

![image-20200531194727226](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531194727226.png)

![image-20200531194803157](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531194803157.png)

![image-20200531194825471](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531194825471.png)



![image-20200531194841983](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531194841983.png)

![image-20200531194934393](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531194934393.png)

![image-20200531194943521](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531194943521.png)

![image-20200531194951434](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531194951434.png)

![image-20200531195003249](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531195003249.png)

![image-20200531195017103](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531195017103.png)

![image-20200531195028502](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531195028502.png)



![image-20200531195119462](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531195119462.png)

# JAVA01

1. 简单
2. 面向对象
3. 可移值
4. 高性能
5. 分布式（web url 就是访问地址
6. 动态性（反射
7. 多线程
8. 安全性
9. 健壮性

## java的成功

- 互联网

## java的三大版本

- javase 标准版（桌面，控制

- ~~javame嵌入式~~

- javaee （web ，服务器

## JDK ,JRE,JWM

1. JDK包含全部开发者工具
2. jre包含运行换环境
3. jvm虚拟机

## 代码

```java
public class Hello{
    publc static void main(String[] args){
        System.out.print("hello");
	}
}
#javac Hello.java
    #java Hello
```

## java 运行机制

- 编译型（java->计算机
- 解释性（用一下编译一下
- 源程序->.class(字节码)

## java的基础语法

- 注释

- ```
  /*
  *                    .-'-._
  *                   /    e<
  *               _.-''';  (
  *     _______.-''-._.-'  /
  *     ====---:_''-'     /  _  _     %%%%
  *              '-=. .-'` _(_)(_)   %%|/%%%
  *                _|_\_  (_)(_)(_) %%%%%%%%%%
  *               //\\//\\//\\//\\//\\%/_%%%%%%%
  *           ____\\//\\//\\//\\//\\// |__|/__%%%
  *  ________(___  \\/\//\\//\\//\\//__//___%%%%%%%
  *            / \  \_/ __ \___//------\--%%%%%%
  *  _________/   \____/  \____/\\%%%%%%%%%%%%
  *                              \_-%%%%%%%%
  *
  */
  
  ```

- 

file Struc

//

/**

*

*/

javadoc

百度有趣的代码注释

## 关键字

程序员

- 变量名只可以字母~~$ 下划线~~~开始 

- ~~中文名~~也可以是变量名

- 标识符号是大小写敏感的

## 数据类型

- （整数）byte：8位，用于表示最小数据单位，如文件中数据，-128~127(一个字节)
  short：16位，很少用，-32768 ~ 32767
  int：32位、最常用，-2^31-1~2^31 （21亿）（4个字节
  long：64位、次常用
- （浮点数）float：32位，后缀F或f，1位符号位，8位指数，23位有效尾数。
  double：64位，最常用，后缀D或d，1位符号位，11位指数，52位有效尾数。（8字节
- 强类型语言（要求变量的类型都必须定义
- 基本类型 int double float short long byte-128-127 
- 浮点数
- long后面加L
- float后面加F
- String不是关键字是一个类
- 引用类型
- 类
- 接口
- 数组

```java
import java.math.BigDecimal;

public class De1 {
    public static void main(String[] args) {
        int i=10;
        int i2=010;//八
        int i3=0x10;//十六
        System.out.println(i);
        System.out.println(i2);
        System.out.println(i3);
        /***********************
         * 银行的价钱
         */
        float f=0.1f;
        double d=1.0/10;
        System.out.println(f==d);
        float d1=2133333333333333f;
        float d2=d1+1;
        System.out.println(d1==d2);
        //不精确的比较 float 是有误差的
        //一定避免使用浮点数进行比较
        //BigDecimal
        char c1='c';
        System.out.println((int)c1);
        //所有的字符本质就是数字
        //unicode 2字节 65536
        //U0000 uffff
        char c3='\u0061';
        System.out.println(c3);
        //转义字符
        System.out.println("hello\tworld\n你好");
        //
        String sa=new String("hello,world");
        String sb=new String("hello world");
        System.out.println(sa==sb);
        System.out.println(sa.equals(sb));
        String sc="hello world";
        String sd="hello world";
        System.out.println(sc==sd);
        System.out.println(sc.equals(sd));
    }
}

```

- char 的本质就是数

## 基础类型转换

---

### byte,short,char->int->long64->float32->double(小数的优先级)

- 强制类型转换（高到低
- 自动转换（低到高

```java
public class Demo3 {
    public static void main(String[] args) {
        int i=128;
        byte b=(byte)i;//强制转换
        System.out.println(i+"  "+b);//128  -128内存溢出、
        /**
         * 1.不能布尔值转换
         * 2.不能把对象转换为不相关
         * 3.低到高强制转换
         * 4.可能存在内存溢出
         */
        System.out.println((int)23.7);//23
        System.out.println((int)-45.89f);
        char c='a';
        int d=c+1;
        System.out.println(d);
        System.out.println((char)d);
        //jdk7可以用下划线分割
        int money=10_0000_0000;
        System.out.println(money);
        int year=20;
        //int total=money*year;
        long total=money*year;//默认抓换为int；
        System.out.println(total);
        long total3=money*(long)year;
        System.out.println(total3);//常见问题
        //L l
        
    }
}

```



## 变量

- 可以变化的量；

- 基本类型      String等引用类型

- 作用域

  ### 变量的类型

  - 类变量  static

  - 实例变量 没有static

  - 局部变量

  - ```
    public class Demo05 {
        static int a=1000;//类变量
        static double salary=25000;
        String name;//实例变量
        public static void main(String[] args) {
            //局部变量在方法里面;声明和初始化
            int i=10;
            //
            Demo05 demo05=new Demo05();
            System.out.println(demo05.name);
            System.out.println(a);
        }
        public void add(){
    
        }
    }
    
    
    ```

    

  ## 常量是不允许改变的

  - fianl static 修饰符号不分顺序

## 命名规范

骆峰原则

常量大小

类首字母大写

变量小写

方法

# JAVA02

## 运算符

1. 算数运算符号 + - * / % ++ --
2. 赋值=
3. 关系 > < >=  <= == != instanceof
4. 逻辑 && || ！
5. 不同的数值类型相加取最大的类型
6. ++ --

```java
package operrator;

public class add {
    public static void main(String[] args) {
        int a=3;
        //++ -- 一元运算符
        int b=a++;
        System.out.println(a);//4
        int c=++a;
        System.out.println(b);//3
        System.out.println(a);//5
        System.out.println(c);//5
        System.out.println(a);//5
        double k=Math.pow(2,3);
        //可以使用工具类
        System.out.println(k);
    }
}

```

- 逻辑运算符

  ```java
  package operrator;
  
  public class Demo06 {
      /**
       * A=0011 1100
       * B=0000 1101
       * A&B 0000 1100
       * A|B 0011 1101
       * A^B 0011 0001/相同为0
       * ~B 1111 0010
       *
       * 2*8=16 2*2*2*2
       *
       * 0000 0001    1
       * 0000 0010    2
       * 0000 0100    4
       * 0000 1000    8
       * /<<右移*2
       * >>左移动/2
       */
      public static void main(String[] args) {
          System.out.println(2<<3);
      }
  
  }
  
  ```

  ```java
  package operrator;
  
  public class T3 {
      public static void main(String[] args) {
          int a = 12;
          int b=34;
          //System.out.println(a+=b);
          System.out.println(""+a+b);
          System.out.println(a+b+"");
          //x? y:z
          int ad=10;
          String kkd=ad< 60?"不及格":"及格";
          System.out.println(kkd);
  
      }
  }
  //()优先级
  ```

  

## 包机制

com.kangsdan.www

阿里巴巴开发手册 [下载地址](https://www.cnblogs.com/han-1034683568/p/7680354.html)代码规范

## java Doc

文档注释

```java
package com.kangsdan.Base.kdd;

/**
 * @author 进哥
 * @version 0.1
 *
 */

public class T1  {
    /**
     *
     * @param args
     * @throws Exception
     */
    public static void main(String[] args) throws Exception{

    }
}

```

javadoc -encoding utf-8 -charset utf-8

-encoding是java代码编码，-charset是对生成文档所用的编码。-windowtitle就是对应html的<title>标签

```
-encoding UTF-8 -charset UTF-8 -windowtitle "test"
```

![image-20200528114111921](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200528114111921.png)

## 基础进阶

### java nextLine的方法

![image-20200528222948336](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200528222948336.png)

```java
package com.kangsdan.Base.operrator;

import java.util.Scanner;

public class Ent {
    public static void main(String[] args) {
        //next
        Scanner ent=new Scanner(System.in);
        String a=ent.next();
        String b=ent.nextLine();
//        System.out.println(a);
//        System.out.println(b);
        //判断有没有字符串输入
        //next输入没办法接受空格 nextLine可以节收空格
        if(ent.hasNext()){
            String kdd=ent.next();
            System.out.println(kdd);
        }
        if(ent.hasNextLine()){
            String zcj=ent.nextLine();
            System.out.println();
        }if(ent.hasNextInt()){
            int kint=ent.nextInt();
            System.out.println(kint);
        }else {
            System.out.println("不是书记");
        }
        //io资源用完就必须关掉
        ent.close();
    }
}

```

```jav
package com.kangsdan.Base.operrator;

import java.util.Scanner;

public class Demo1 {
    public static void main(String[] args) {
        Scanner scanner=new Scanner(System.in);
        double sum=0;
        int m =0;
        while (scanner.hasNextDouble()){
            double x=scanner.nextDouble();
            m++;
            sum=x+sum;
        }
        System.out.println("计算结果 "+sum);
        scanner.close();
    }
}

```

## 流程控制

- 顺序 

```java
package com.kangsdan.Base.operrator;

public class ShunXuDemo {
    public static void main(String[] args) {
        System.out.println("1");
        System.out.println("2");
        System.out.println("3");
        System.out.println("4");
        System.out.println("5");
    }
}

```



- 选择 if 单双多嵌套 switch

```java
package com.kangsdan.Base.operrator;

import java.util.Scanner;

public class ShunXuDemo {
    public static void main(String[] args) {
        Scanner scanner=new Scanner(System.in);
        System.out.println("输入");
        String a=scanner.nextLine();
        if(a.equals("a")){
            System.out.println("我是一个中国人");
        }else if(a.equals("kdd")){
            System.out.println("中国nb");
        }else if(a.equals("zcj")){
            System.out.println("中国fashion");
            if(a.equals("1")){
			}
        }
//出来就可以
        scanner.close();
    }
```

```java
package com.kangsdan.Base.operrator;

import java.util.Scanner;

public class ShunXuDemo {
    public static void main(String[] args) {
    Scanner scanner=new Scanner(System.in);
    char gread='c';
//字符的本质还是数
    switch (gread){
        case 'c':
            System.out.println("good");
            break;
        case 'b':
            System.out.println("very");
    }
    scanner.close();
    }

}

```

![image-20200528230010864](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200528230010864.png)

- 循环（day3
- 控制

```java

```



# JAVA03

## Java的反编译idea

- 将字节码文件拖到idea的工作目录，必须在文件的形式下，不能直接拖到idea。然后直接打开就是。class的反编译的文件
- 看源码是一个好的习惯

## 循环结构

- while 

```java
package com.kangsdan.Base.operrator;

public class WhileDemo01 {
    public static void main(String[] args) {
        int i=0;
        int sum=0;
        while(i<=100){
            System.out.println(i);
            sum=i+sum;
            i++;
//sum=i+sum;(如果在下面的结果为5151；就是错误的，你要加的对象是谁，是不是错误了
        }
        System.out.println(sum);
    }
}
//先判断，后执行
```



- do ..while

```java
package com.kangsdan.Base.operrator;

public class WhileDemo01 {
    public static void main(String[] args) {
        int i=0;
        int sum=0;
        do{
            sum+=i;
            i++;//迭代
        }while (i<=100);
        System.out.println(sum);
    }
}
//先执行后判断，至少跑一次
```



- while ..do
- for

```java
package com.kangsdan.Base.operrator;

public class WhileDemo01 {
    public static void main(String[] args) {
       // int i=0;
        int sum=0;
        int sum2=0;
        //   初始     布尔       迭代
        for (int i = 0; i <=100 ; i++) {
            //都可以删除
            if(i%2==0){
                sum+=i;
            }
            //0到100之间奇数和偶数和
            if (i%2!=0){
                sum2+=i;
            }
        }
        //100.for快捷键

        System.out.println("over "+sum+sum2);//字符串在前就全为字符串
    }
}
//java输出奇数偶数和
```

```java
package com.kangsdan.Base.operrator;

public class WhileDemo01 {
    public static void main(String[] args) {
        for (int i = 0; i < 1000; i++) {
            if(i%5==0){
                System.out.print(i+"\t");

            }
            if(i%(5*3)==0){
                System.out.println();
            }
        }
    }
}
//能被5整除，每3个换一个
```

```java
public class WhileDemo01 {
    public static void main(String[] args) {
        for (int i = 1; i < 10; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print(j+"*"+i+"="+(i*j)+"\t");
            }
            System.out.println();
        }

    }
}
//九九乘法表

```

- 增强for循环

```java
public class WhileDemo01 {
    public static void main(String[] args) {
       int[] num={10,20,40,50};//数组
        for (int i:num) {
            System.out.println(i);
        }
    }
}
//遍历数组的内容 集合
//增强for循环
```

- break；continue

```java
public class WhileDemo01 {
    public static void main(String[] args) {
       int i=0;
       while(i<100){
           i++;
           if(i==30){
               break;//强制退出循环
           }
       }
        System.out.println(123);
    }
}
```

```java
public class WhileDemo01 {
    public static void main(String[] args) {
       int i=0;
       while(i<100){
           i++;
           if(i%10==0){
               continue;//回到起点
           }
           System.out.println(i);
       }
        System.out.println(123);
    }
}
```

- 强制退出break 每个地方
- continue 只可以用到循环中

## ~~goto~~

java 没有得到正式使用，唯一用到标签的时候 循环

```java
public class WhileDemo01 {
    public static void main(String[] args) {
       int count=0;
        outer:for (int i = 101; i < 150; i++) {
            for (int j = 2; j <i/2 ; j++) {
                if(i%j==0) {
                    continue outer;
                }
            }
            System.out.println(i+"\t");
       }
    }
}
//只是一个标签
```

## 流程控制练习

```java
public class Demo {
    //打印三角形
    public static void main(String[] args) {
        for (int i = 1; i <=5 ; i++) {
            for (int j = 5; j >= i; j--) {//拆分，这是一个好的方式
                System.out.print(" ");
            }
            for (int j = 1; j <=i; j++) {
                System.out.print("-");
            }
            for (int j = 1; j <i; j++) {
                System.out.print("-");
            }
            System.out.println();
        }
    }
}
//拆分的思想
```

## Java的方法

- **什么是方法**

```java
public class T1 {
    public static void main(String[] args) {
       //main 方法
        int a=new T1().add(1,2);
        System.out.println(a);
    }
    //修饰符 返回类型 方法名 参数
    public int add(int a,int b){
        return  a+b;//返回 终止方法
    }
}
```



1. System是一个类 out 对象 println方法
2. 方法是语句的集合
3. 方法在类 或者对象中
4. 在程序创建其它地方调用
5. 原子性:一个方法完成一个功能

- **方法的定义**

1. 一段完成特定功能的代码

2. 方法包含一个方法名和方法体

3. 修饰符public 返回值 方法名 参数类型 方法体

4. java是值传递（max  引用传递

5. ## 内存模型

6. ![img](https://img-blog.csdnimg.cn/20190320020844580.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3hpYW9qaW5sYWkxMjM=,size_16,color_FFFFFF,t_70)

- **方法重载**

1. 同一个类中参数不同的方法（相同的名字，参数不同
2. 名字不同 参数不同 个数顺序 
3. 返回类型  不限制
4. 他会自动匹配

```java
public class T2 {
    public static void main(String[] args) {

    }
    public static  int add(int a,int b){
        return a+b;
    }
    public  static int add(int a){
        return 2*a;
    }

}
//方法的重载
```



- **命令行传参**

将ming'li

![image-20200529202224912](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200529202224912.png)

- **可变参数**

1. jdk1.5开始
2. 在指定参数类型后+...
3. 只能一个可变参数而其必须在最后

```java
public class Demo04 {
    public static void main(String[] args) {
        new Demo04().test(1,4,5);
    }
    public void test(int...i){
        for (int j = 0; j <i.length ; j++) {
            System.out.println(i[j]);
        }
        System.out.println(i[0]);
    }

}
//可变参数 本质就是数组可以传递数组
```

- ***递归***（能不用就他丫的不用，影响效果）

  1.自己调用自己

  2.递归头

  3.递归体

  ```java
  public class DE0 {
      public static void main(String[] args) {
          System.out.println(new DE0().test(5));
      }
      public int test(int n){
          if(n==1){
              return 1;
          }else{
              return n*test(n-1);
          }
      }
  }
  //递归方法
  ```

  ![image-20200529203825805](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200529203825805.png)

//递归的方法

边界条件 （1）

前阶段

返回阶段

**java是使用栈基址的**

调用方法压栈。

# JAVA04



## 数组

- 概念

  1.相同类型数据集合

  2.可以通过下标访问
  ![image-20200530201228781](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200530201228781.png)

  ![image-20200530195736912](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200530195736912.png)

- 声明

```java
import java.util.Scanner;

public class Demo01 {
    //变量类型   变量名=变量值;
    public static void main(String[] args) {
        int[] nums;//定义
        int sum=0;
        int nums2[];//效果相同但不推荐  c/c++的
        //dataType[] a=new dataType[arrayLength];
        nums=new int[10];
        Scanner scanner=new Scanner(System.in);
        for (int i = 0; i <nums.length ; i++) {
            nums[i]=i+1;
            sum+=nums[i];
            System.out.print(nums[i]+" ");
        }
        System.out.println("求和结果 "+sum);
    }
}
//array.length
```

### 内存分析

1. **堆**  new对象 数组   线程共享，不会存放别的对象引用
2. **栈** 基本变量类型（包含具体的数值  引用对象的变量指向具体值的堆地址
3. **方法区** 所有线程共享 包含所有的class static  类和class是同时产生的

- 使用
- 多维数组

```java
java.lang.ArrayIndexOutOfBoundsException//数组越界错误
```

```java
public class Demo02 {
    public static void main(String[] args) {
        //静态初始化
        int[] a={1,2,3,4,5};//创建加值就是初始化
        Man[] mans={new Man(),new Man()};
        //动态初始化
        int[] b=new int[10];//默认为0
    }
}
```

## 特点

1. 长度是确定的
2. 类型相同
3. 可以包括基本和引用
4. 数组是对象，原始还是其它都在堆
5. [0]->[length-1]

## 使用

```java
public class Demo02 {
    public static void main(String[] args) {
        //静态初始化
        int max=0;
        int[] a={1,2,3,4,5,3};//创建加值就是初始化
        for (int i:a) {
            System.out.println(i);
        }
        for (int i = 0; i < a.length; i++) {
            if(a[i]>max){
                max=a[i];
            }
        }
        kdd(a);
        System.out.println(max);
    }
    public static void kdd(int...i){
        System.out.println("反转开始");
        int j=0;
        int d=(i.length)-1;
        int[] res=new int[i.length];
        while (d!=0) {
            res[j++] = i[d--];
        }
        for (int i1 = 0; i1 < res.length; i1++) {
            System.out.print(res[i1] + " ");
        }
        System.out.println("反转结束");
    }
}
```

## 多位数组

```
//int[][] a=new int[][];
```

![image-20200530204240090](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200530204240090.png)

```java
package com.kangsdan.Base.ArrayT;

public class Demo03 {
    public static void main(String[] args) {
        int[][] a=new int[3][3];
        for (int i = 0; i < a.length; i++) {
            for (int i1 = 0; i1 < a[i].length; i1++) {
                a[i][i1]=i+1;
                System.out.print(a[i][i1]+" ");
            }
            System.out.println();
        }
        System.out.println(a.length);//3
        System.out.println(a[0].length);//3
    }
}

```

## Arrays类

1.java.util.Arrays;工具类

```java
public class Damo04 {
    int[] a={1,898,5,3,456,65,61256,45};//没有在下面起到作用

    public static void main(String[] args) {
        int[] a={1,898,5,3,456,65,61256,45};
        for (int i:a) {
            System.out.println(i);
        }
    }
}
```

```java
import java.util.Arrays;

public class Damo04 {
    int[] a={1,898,5,3,456,65,61256,45};

    public static void main(String[] args) {
        int[] a={1,898,5,3,456,65,61256,45};

//        for (int i:a) {
//            System.out.println(i);
//        }
        Arrays.sort(a);//排序
        System.out.println(Arrays.toString(a));//打印内容
        System.out.println(Arrays.binarySearch(a,5));//排好序的查找，返回下标
        int[] b=new int[8];
        Arrays.fill(b,20);
        if(Arrays.equals(a,b)){
            System.out.println("这两数值一模一样");
        }else {
            System.out.println("抱歉，不相同");
        }


        Arrays.fill(a,20);//赋值
        System.out.println(Arrays.toString(a));
        if(Arrays.equals(a,b)){
            System.out.println("这两数值一模一样");
        }

    }
}
// Arrays.fill(b,2,4,20);
```

## 冒泡排序法

```java
public class Demo07 {
    public static void main(String[] args) {
        int[] a={9,4,6,5,7,3};
        int temp=0;
        for (int i = 0; i < a.length-1; i++) {
            for (int j = 0; j <a.length-1 ; j++) {
                if(a[j]>a[j+1]){
                    temp=a[j];
                    a[j]=a[j+1];
                    a[j+1]=temp;
                }
            }
        }
        for (int i:a
             ) {
            System.out.println(i);
        }
    }
}
//江湖人都知道的冒泡排序法
```

- 时间复杂度是O（n^2)

## 稀疏数组

```java

```

1. 大部分是0
2. 计算多少行列  不同的元素
3. ![image-20200530215746062](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200530215746062.png)

```java
public class Demo05 {
    public static void main(String[] args) {
        //定义一个二维数组 0无 1黑 2白
        int[][] a=new int[11][11];
        a[1][2]=1;
        a[2][3]=2;
        for (int[] ints:a){
            for (int i:ints) {
                System.out.print(i+"\t");
                if(i!)
            }
            System.out.println();
        }
        //转化稀疏数组
        //获取有效值的个数
        int sum=0;
        
    }
}
//原始
```

```java
public class Demo05 {
    public static void main(String[] args) {
        //定义一个二维数组 0无 1黑 2白
        int[][] a=new int[11][11];
        a[1][2]=1;
        a[2][3]=2;
        int sum=0;
        for (int[] ints:a){
            for (int i:ints) {
                System.out.print(i+"\t");
                if(i!=0){
                    sum++;
                }
            }
            System.out.println();
        }
        //转化稀疏数组
        //获取有效值的个数
        //创建稀疏数组
        int[][] arr2=new int[sum+1][3];
        arr2[0][0]=11;
        arr2[0][1]=11;
        arr2[0][2]=sum;
        int count=0;
        for (int i = 0; i < a.length; i++) {
            for (int j= 0; j < a[i].length; j++) {
                if(a[i][j]!=0){
                    count++;
                    arr2[count][0]=i;
                    arr2[count][1]=j;
                    arr2[count][2]=a[i][j];

                }
            }
        }
        System.out.println("这个就是"+count);
        for (int i = 0; i <arr2.length ; i++) {
            System.out.println(arr2[i][0]+"\t"+arr2[i][1]+"\t"+arr2[i][2]);
        }
    }
}
```

```java
import java.util.Arrays;

public class Demo05 {
    public static void main(String[] args) {
        //定义一个二维数组 0无 1黑 2白
        int[][] a=new int[11][11];
        a[1][2]=1;
        a[2][3]=2;
        int sum=0;
        for (int[] ints:a){
            for (int i:ints) {
                System.out.print(i+"\t");
                if(i!=0){
                    sum++;
                }
            }
            System.out.println();
        }
        //转化稀疏数组
        //获取有效值的个数
        //创建稀疏数组
        int[][] arr2=new int[sum+1][3];
        arr2[0][0]=11;
        arr2[0][1]=11;
        arr2[0][2]=sum;
        int count=0;
        for (int i = 0; i < a.length; i++) {
            for (int j= 0; j < a[i].length; j++) {
                if(a[i][j]!=0){
                    count++;
                    arr2[count][0]=i;
                    arr2[count][1]=j;
                    arr2[count][2]=a[i][j];

                }
            }
        }
        System.out.println("这个就是"+count);
        for (int i = 0; i <arr2.length ; i++) {
            System.out.println(arr2[i][0]+"\t"+arr2[i][1]+"\t"+arr2[i][2]);
        }
        System.out.println("还原");
        int[][] arr3=new int[arr2[0][0]][arr2[0][1]];
        //还原值
        for (int i = 1; i < arr2.length; i++) {
            arr3[arr2[i][0]][arr2[i][1]]=arr2[i][2];
        }
        for (int i = 0; i <arr3.length ; i++) {
            System.out.println(Arrays.toString(arr3[i]));
        }

    }
}
//稀疏数组的完结版
```

# JAVA 05

- Oop面向对象编程
- oo面向对象
- 面向对象&面向过程
- 1. 物以类聚（分类、对某个分类进行独立的思考->框架
- ​    2.步骤清晰简
- 面向对象本质：类的方式组织代码，对象的方式组织（封装）数据;
- 抽象->xiang
- 三大特性
  1. 封装
  2. 继承
  3. 多态

- 认识的角度现有对象然后又类，类是抽象的，是对对象的抽象
- 代码运行的角度是先有类再有对象，对象是类的模板

##  方法

```java
import java.io.IOException;

//类
public class Demo01 {
    //main方法
    public static void main(String[] args) {
        new Demo01().lov();
    }
    /*
    修饰符 返回值 方法名（参数）
    //方法体
    return 返回值
     */
    public String sayHello(){
        return "heoo";
    }
    public void lov(){
        System.out.println("I love you kdd");
        return;
    }
    public int max(int a,int b){
        int c;
        return a>b?a:b;
    }
    /*
    brak switch  结束循环     return 结束方法返回结果
     */
    public void readFile(String file)throws IOException{
        
    }

}
```

//导入的是包;

```java
//学士类
public class Student {
    //方法
    //类实例化之后才会存在
    public void say(){
        System.out.println("学生说话了");
    }
    //和类一起加载的
    public static void a(){
        //say();
    }

}
```

```java
public class Demo02 {
    //静态方法 static
    //非静态方法
    public static void main(String[] args) {
        new Student().say();
    }
}
```

## 值传递

```java
//值传递
public class Demo04 {
    public static void main(String[] args) {
        int a=1;
        Demo04.change(a);
        System.out.println(a);
    }
    public static void  change(int a){
        a=10;
    }
}
```

```java
//引用传递 对象  本质还是值传递
public class Demo05 {
    public static void main(String[] args) {
        Person person = new Person();
        Person person1 = new Person();
        System.out.println(person.name);
        person.name="康丹丹";
        System.out.println(person.name);
        System.out.println(person1.name);
    }
}
//定义一个Person类 一个属性 name
class  Person{
    String name;//null;
}
```

## 对象 

- 共同特征的事务抽象的（类
- 具体的实例（对象
- New关键字创建对象

```java
//一个项目只有一个main方法
public class Application {
    //类抽象实例化对象
    public static void main(String[] args) {
        //student是Studdent的对象
        Student student = new Student();
    }
//对世界更好的建模  音乐
}
//面向对象  类的方式组织代码，对象的方式封装数据
```

```java
package com.kangsdan.Base.OOp;
//学士类
public class Student {
    //属性
    String name;
    //方法
    //类实例化之后才会存在
    public void say(){
        System.out.println("学生说话了");
    }
    //和类一起加载的
    public static void a(){
        //say();
    }

}

```

### 构造器

- 构造方法

![image-20200531110907332](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531110907332.png)

1.必须与类名相同 类型为空

```java
public class Person {
    //一个类上面都没有也会存在方法
    //显示定义的构造器
    //实例化创建
    //使用new关键字必须有构造器，本质就是调用构造器
    public Person(){
        System.out.println("hello");
    }
    //创建了有参构造必须有无参
    public Person(String name){//重载

    }
    //alt+ins快捷键
}
```

### *构造器*

1. 相同
2. 无返回
3. 初始
4. new 本质就是调用构造器方法
5. 想使用有参必须显式定义一个无参构造
6. this.当前类的东西





## 内存的简单分析

常量直接在栈里面

![image-20200603171848614](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200603171848614.png)

<img src="C:\Users\1\Desktop\日记\无标题.png" alt="无标题" style="zoom:200%;" />

```java
/**
 * 类是一个模板 对象是具体的实例
 * 类是抽象的 对象是具体
 * 定义 与调用
 * 引用类型 除基本类型都是影响，对象是通过是引用操作的
 * 对象是通过是引用来操作的  栈-》堆中
 * 对象属性 -》字段 成员变量 属性和
 * 属性会有默认的初始化
 * 数值 0 0.0
 * char u0000
 * boolea false
 * 引用null
 * 基本类型 8；
 * 修饰符 类型 属性名 值
 * 方法
 *
 * 对象的创建和使用
 * 必须用new
 * 构造器
 * 对象的属性     Person per =new Person(); per.name; per.sleep();
 * 类是
 *  静态的属性 操作
 *  动态的属性 方法
 ** **封装 继承 多态
 */
```



## 封装

- 高聚合  低耦合（内部细节是自己完成的，不允许外部干涉，低耦合 ：仅暴露少量的方法给外部使用
  1. 电视机 提供接口

- 禁止访问对象中的实际数据 应该通过接口来访问
- 私有属性 get set

```java
public class T1 {
    //私有属性
    private String name;
    private int id;
    private char sex;
//获得属性（字段
    public String getName() {
        return name;
    }
//设置属性 （字段
    public void setName(String name) {
        this.name = name;
    }

    public int getId() {
        return id;
    }

    public void setId(int id) {
        this.id = id;
    }

    public char getSex() {
        return sex;
    }

    public void setSex(char sex) {
        this.sex = sex;
    }
}
```

```java
public class Appliction {
    static int[] a=new int[10];
    public static void main(String[] args) {
        //实例化对象
        T1 t1 = new T1();
        t1.setName("康丹");
        System.out.println(t1.getName());

    }
}
```

- 通过get和set 就可以保证安全
- 保护数据，隐藏代码的细节
- 统一接口
- 提高了系统的维护性

###  重载（复习

实现；

//方法 参数都相同都是方法

## 继承

- 继承是对一批类的抽象 ，实现 父类的扩展
- extends 扩展 ，子类是父类的扩展
- java中只有单继承 没有多继承（一个儿子只有一个爸爸，一个爸爸几个儿子
- 继承是类和类之间的一种关系   （还有组合 聚合 依赖
- 子类 派生类 父类 基类 extends
- is a的关系

```java
package com.kangsdan.Base.Exten;
//这是一个类 人
//public
//protected
//default
//private
public class Person {
    public int mon=1000_121;
    public void say(){
        System.out.println("说了一句话");
    }
//ctrl+h可以显示继承表
    
}

```

```java
package com.kangsdan.Base.Exten;

public class Student extends Person{
//子类继承了父类就有他的全部方法
    //123_444
}

```

```java
package com.kangsdan.Base.Exten;

public class Appliction {
    public static void main(String[] args) {
        new Student().say();
    }
}

```

```jav
package com.kangsdan.Base.Exten;
//学生是人  派生类
public class Teacher extends Person{

}

```



- object类
- ![image-20200531151158617](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200531151158617.png)

## 在java中默认继承object

- 贯穿java



## super

```java
package com.kangsdan.Base.Exten;

public class Student extends Person{
//子类继承了父类就有他的全部方法
    //123_444
    private String name="老赵";
    public void test(String name){//kd
        System.out.println(name);//kd
        System.out.println(this.name);//老赵
        System.out.println(super.name);//进
    }
}
//没有关键字调用本方法
 //this调用 类方法
//super继承 父类
```

```java
package com.kangsdan.Base.Exten;
//这是一个类 人
//public
//protected
//default
//private
public class Person {
    protected String name="进";
    public int mon=1000_121;
    public void say(){
        System.out.println("说了一句话");
    }
//ctrl+h可以显示继承表

}

```

```java
package com.kangsdan.Base.Exten;

public class Appliction {
    public static void main(String[] args) {
        Student person = new Student();
        person.test("kd");
    }
}

```

//私有的属性没办法继承

```java
public class Person {
    public Person(){
        System.out.println("Person");
    }

}
package com.kangsdan.Base.Exten;

public class Student extends Person{
//子类继承了父类就有他的全部方法
    //123_444
    public Student(){
        super();//有产必须有参
        System.out.println("student");
    }

}
package com.kangsdan.Base.Exten;

public class Appliction {
    public static void main(String[] args) {
        Student person = new Student();
//Person
//student
//默认就吊用了父类的构造方法 调用父类的构造器必须在子类的第一行
    }
}



```

1. super 调用夫类的构造方法必须在第一个

2. super 必须在子类的构造方法 或者方法中 否则就是object的
3. super和this不能同时调用构造方法
4. this代表本身   super 调用父类 
5. this  上面时候都可以
6. super 继承 
7. this（）本类的构造
8. 父类的构造

- 方法

## 方法的重写-->多态

- 重写只和静态方法有管，和非静态方法无关

```java
public class Demo02 {
    public void test(){//static的方法是没有办法重写的
        System.out.println("B");
    }
}

public class Demo01 extends Demo02{
    @Override
    public void test() {
        super.test();
    }
}

public class Appliction {
    //方法的调用与定义的类型有关
    public static void main(String[] args) {
        new Demo01().test();//走Demo01
        Demo02 demo02 = new Demo01();
        //父类指向了子类  static的方法才是这样的本身static不是继承
        demo02.test();//走Demo02
    }
}
```

### 总结

- 重写：需要有继承关系 。子写夫
-  方法 参数列表 必须相同
- 可以放大 博客与缩小 修饰符
- public》protected》default 》private
- 异常范围可以缩小不可以扩大
- ClassNotFound-->Exception
- **方法相同，方法体不同**

### 为什么需要重写

父类的功能 子类不一定需要

# JAVA06



## 多态

- 动态编译：类型 可拓展性更强
- **一个对象实际类型的确定的   引用类型不确定**
- Person a=new Student();
- Studen b=new Student();
- Object c=new Student();

```java
public class Person {
    public void eat(){
        System.out.println("eat");
    }

}

public class Student extends Person{
    @Override
    public void eat() {
        System.out.println("s");
    }
    public void run(){
        System.out.println("run");
    }

}

public class Main {
    public static void main(String[] args) {
        Student student=new Student();
        Person person=new Student();
        Object object=new Student();
        //person.run();
        ((Student)person).run();//高转低
        //子类可以调用父类的方法重写后调用子类的
        //类型是父类没有的方法不能调用子类的方法
    }
}
```



1. 多态面向的是方法 属性和字段没有方法
2. 父类和子类之间有关系   类型转换异常 ClassCastException
3. 首先得有继承关系   存在复写
4. 父类引用指向子类



- Static 与类不能
- Finall不能
- private也不能重写

## instanceof 类型转换

```
// x instanceof y->存在父子关系
public class Main {
    //Object
    //Object>Person>Studen
    public static void main(String[] args) {
        Object object = new Student();
        System.out.println(object instanceof  Object);//true
        System.out.println(object instanceof Student);//true
        System.out.println(object instanceof Person);//true
        System.out.println(object instanceof String);//false

        Student object1 = new Student();
        System.out.println(object1 instanceof  Object);//true
        System.out.println(object1 instanceof Student);//true
        System.out.println(object1 instanceof Person);//true
        //System.out.println(object instanceof String);//false同节无法比较
    }
}
```

- 类型转换 父类高 只类低  低转高是自动完成的   高转低要i强制转换

- 子类转父类可能会丢失一些方法

- 父类指向子类对象

- 子类->父类向上

- 父类 子类 向下强制转换

- ## 抽象的思想

## Static 

- 静态方法 
- 静态属性

```java
package com.kangsdan.Base.zcj;


public class Demo07 {
    private static int age;//静态
    private double score;//非静态
    public void say(){
        System.out.println("say");
    }
    public static void run(){
        System.out.println("run");
    }
    public static void main(String[] args) {
        new Demo07().say();//非静态调用
        Demo07.run();//静态调用
        Demo07 student=new Demo07();
        System.out.println(student.score);
        System.out.println(student.age);
        System.out.println(Demo07.age);//静态变量 共享
        //System.out.println(Demo07.score);

    }
}

```

## 静态方法 静态代码块 构造方法



```java
package com.kangsdan.Base.zcj;

public class Demo {
    {//可以给初始值
        System.out.println("匿名代码块");
        //代码块
    }
    static {//只执行一次
        System.out.println("静态代码块");
        //静态代码块
    }
    public Demo(){
        System.out.println("构造方法");
    }

    public static void main(String[] args) {
        new Demo();
        System.out.println("***************");
        new Demo();
    }
}

```

- 静态导入包

```java
import static java.lang.Math.random;//静态导入包
public class Dem0{
    public static void main(String[] args) {
        System.out.println(random());
    }
}
```

- final 无法继承



## 抽象类

- abstract

```java
public abstract class Action01 {//抽象类
    //约束 有人帮实现
    //只有方法名没有方法提
    //继承就必须重写
    //不能new出来
    //只能靠子类复写
    public abstract void doSomthing();
}
```

- 接口可以实现多继承（Java没有多继承

- ```java
  public abstract class Action01 {//抽象类
      //约束 有人帮实现
      //只有方法名没有方法提
      //继承就必须重写
      //不能new出来
      //只能靠子类复写
      //抽象的方法可以有普通的类
      //抽象的类必须在抽象的方法
      public abstract void doSomthing();
  }//提高开放效果
  ```

- 关于抽象类有没有构造器 [连接](https://blog.csdn.net/qq_40728375/article/details/79890223)、

```java
以举例的方式说到如何区分抽象类和接口，这里我们从Java语法谈起，使我们更加了解这两者的内在区别。它们的语法区别：
1）接口不能有构造方法，抽象类可以有。
2）接口不能有方法体，抽象类可以有。
    3）接口不能有静态方法，抽象类可以有。
    4）在接口中凡是变量必须是public static final，而在抽象类中没有要求。
————————————————
版权声明：本文为CSDN博主「lllllzllll」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/qq_40728375/article/details/79890223
```

## 接口

- 普通类  只有具体的实现
- 抽象类 具体 和抽象方法
- 接口 只有规范 没有自己的方法 专业的约束 约束和实现分离
- 接口的本质是契约

```java
package com.kangsdan.Base.Demo09;

public interface TimeServeers {
    //属性都是常量  fianl static public
    int age =99;
    void timeSet();
}


public interface UserService {
   //接口中所有的东西都是抽象的 public
    void add(String name);
    void delet(String name);
}


package com.kangsdan.Base.Demo09;
//实现接口的类必须重写方法
public class UserServiceImpl implements UserService ,TimeServeers{
    @Override
    public void add(String name) {

    }

    @Override
    public void delet(String name) {

    }

    @Override
    public void timeSet() {

    }
}

//架构的创建系统 就是用接口定义框架
```

- 总结

1. 约束
2. 定义方法 不同实现
3. 方法类型 public abstract
4. 属性 public static fianl
5. 不能被实例化 没有构造方法
6. 可以实现多个接口，必须要重写接口的方法

## 内部类

- 定义在类内部类

1. 成员内部类
2. 静态内部类（加static
3. 局部内部类（方法内定义的
4. 匿名内部类![image-20200601111914445](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200601111914445.png)

```java
package com.kangsdan.Base.Demo10;

public class Outer {
    private int id;
    public void out(){
        System.out.println("out");
    }
    public class Inner{
        public void inter(){
            System.out.println("inner");
        }
    }

}


package com.kangsdan.Base.Demo10;

public class Appliction {
    public static void main(String[] args) {
        Outer outer=new Outer();
        outer.out();
        //外部类实例化内部类
        Outer.Inner inner=outer.new Inner();
        inner.inter();
    }
}
//可以获取外部类的私有属性 
//一个java 类可以有多个class 只可以有一个public
```

## 异常机制

- Exception
- 文件打开 内存
- 检查性异常 打开不存在的文件夹
- 运行时候异常 在编译时可能被忽略
- 错误 错误不是异常 ERROR堆栈溢出 编译找不到（虚拟机 与程序无关 是虚拟机导致的

![image-20200601154023543](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200601154023543.png)

ArithmeticException：算数异常

```java
public class T1 {
    public static void main(String[] args) {
        int a=1;
        int b=0;
        try {//监控区域
            System.out.println(a/b);
        }catch (ArithmeticException e){//捕获异常
            System.out.println("你输入的数据存在就算错误");
            System.out.println(e);
        }finally {//终究会被执行
            System.out.println("处理完成");
        }
//System.exit(0);
    }
}//快捷键 ctrl+alt+t
```

## throw(s)

```
public class Test2 {
    public static void main(String[] args) {
        int a=10;
        int b=0;
        if(b==0){
            throw new ArithmeticException();//主动抛出异常
        }
    
    }
    public void test()throws Exception{
        
    }
}
```

## 自定义异常

- 

- ```java
  package com.kangsdan.Base.Exception;
  //自定义的异常类
  //双击shfit 就可以搜索类
  public class MyException extends Exception{
  //传递数值》10
      private int detal;
  
      public MyException( int detal) {
          this.detal = detal;
      }
  
      @Override
      public String toString() {
          return "MyException{" +
                  "detal=" + detal +
                  '}';
      }
  }
  
  ```

- 

```java
package com.kangsdan.Base.Demo11;

public class T1 {
    public static void main(String[] args) {
        int a=1;
        int b=0;
        try {//监控区域
            System.out.println(a/b);
            new T1().a();
        }catch(ArithmeticException e){//先小后大否者会被覆盖
            System.out.println("a");
        }
        catch (Throwable e){//捕获异常
            //增加处理异常的代码块
            System.out.println("你输入的数据存在就算错误");
            System.out.println(e);

        }finally {//终究会被执行
            System.out.println("处理完成");
        }

    }
    public void a(){
        a();
    }public void b(){
        b();
    }
}

```

## 经验总结

- 规避和辅助 try—catch
- 多重catch最后写一个最大的异常
- 不确定的代码 加上try catch又可以避免
- 处理异常而不是简单的输出
- 根据业务的需求区确定异常的
- 最后用fianlly来释放占用的资源
- //alt+enter可以提示

# Java se总结

- Java语言的历史
- 博客
- MarkDown语法
- dos命令
- 发展史
- Java诞生1995  c++--
- javase  Javame javaee
- 2006 大数据 Hadoop
- Jdk开发者工具包 jre运行环境



- hello world 开始关系

```java
public class Hello{
    public static void main(String[] args){
        Sytem.out.println("Hello,world");
    }
}
//javac Hello.java
//java Hello
```

- 编译解释语言 



- ```java
  基础语法  行类//    多行/**/    文档注释/** */ 
  ```

- 

- 脚本数据类型 8  整数byte1 short2 int4 long8 浮点数   float4 Double8 字符char2 布尔 boolean1位

- 类栈->堆 接口 数据

0b

0x

0





- 类型转换 自动 子->父  强制



- 变量和常量---

| Final 常量MAX_AD     |      |      |
| -------------------- | ---- | ---- |
| 实例变量  类无static |      |      |
| 类变量 static        |      |      |
| 局部变量 方法        |      |      |

- 规范驼峰（变量方法
- 类首字母大写



- 运算符
- ![image-20200601172701866](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200601172701866.png)





## 包机制

![image-20200601172800461](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200601172800461.png)

### JavaDoc

![image-20200601172842440](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200601172842440.png)

## 流程控制

![image-20200602080342443](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602080342443.png)

## 方法

![image-20200602080732173](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602080732173.png)

- 力扣刷题
- ![image-20200602080931310](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602080931310.png)

## 排序（待学习

![image-20200602081231461](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602081231461.png)

![image-20200602081242690](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602081242690.png)

- 面向对象

![image-20200602081438853](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602081438853.png)

zQQ

![image-20200602081600424](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602081600424.png)

![image-20200602081734661](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602081734661.png)

![image-20200602081805382](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602081805382.png)

![image-20200602081831707](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602081831707.png)

![image-20200602082027358](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602082027358.png)

![image-20200602082103438](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602082103438.png)

![image-20200602082146538](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602082146538.png)

![image-20200602082219588](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602082219588.png)

![image-20200602082306712](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602082306712.png)

- 常用类

![image-20200602082339813](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200602082339813.png)

# 刷题

https://leetcode-cn.com/

# Java07

## 网址

- 未学习：常用类

https://www.bilibili.com/video/BV15W411Z7Wn?from=search&seid=34019508590323883

- 数组

https://www.bilibili.com/video/BV1T4411A7Fy?from=search&seid=5470947643781797232



- 集合框架

https://www.bilibili.com/video/BV1n64y1T7Pk?from=search&seid=7994532544102033516

https://www.bilibili.com/video/BV1eW411R7jx/?spm_id_from=trigger_reload

- java io

https://www.bilibili.com/video/BV1g4411H7Xj?from=search&seid=17485136503942659585

## 数组与排序

- 可以储存相同的数据类型 引用类型
- 必须初始化 分配空间 给出初始化值
- 动态 静态

```java
public class Demo01 {
    public static void main(String[] args) {
        //动态 我们指定长度 系统给值
        int[] a=new int[10];
        //静态 相反
        int[] a1={1,8,9,45,3};
        //取值和赋值  会被分配角标 索引
        int b=a[0];
        //索引给值
        a[0]=99;
    }
}
```

- 常见操作  最大 最小

- ```java
  package com.kangsdan;
  
  public class ArrayDemo {
      public static void main(String[] args) {
          int[] array={1,2,3,4,5,6};
          int temp=0;
          try {
              for (int i = 0; i <array.length; i++) {
                  if(array[i]>temp){
                      temp=array[i];
                  }
                  System.out.println(array[i]);
              }
          } catch (Exception e) {
              System.out.println("越界了");
          }
          for (int i = array.length-1; i >0 ; i--) {
              System.out.println(array[i]);
          }
      }
  
  }
  
  ```

- 反转

```java
public class Change {
    public static void main(String[] args) {
        int[] arrays={1,2,3,4,5,6};
        int temp=0;
        int j=arrays.length-1;
        for (int i = 0; i < arrays.length/2; i++) {
            temp=arrays[i];
            arrays[i]=arrays[j];
            arrays[j--]=temp;//可以通过length-i-1；
        }
        for (int i = 0; i < arrays.length; i++) {
            System.out.print(arrays[i]+" ");
        }
    }
}
```

- 二维数组

```java
public class Demo02 {
    //元素是一维数组的数组
    public static void main(String[] args) {
        int[][] arr2 = new int[][]{{1, 2, 3}, {2, 4, 6}};
        System.out.println(arr2[0][0]);
        int[] a = new int[]{1, 5, 6};
        int[][] arr=new int[3][3];
        System.out.println(arr);
        System.out.println(arr[0]);
        System.out.println(arr[0][2]);
        int[] g,z[] = new int[0][3];
        int b=z[0][0];
    }
}

```

```java
public class YngHui {
    public static void yangHui(int a){
        int[][] kdd=new int[a][a];
        for (int i = 0; i < a; i++) {
            kdd[i][0]=1;
            kdd[i][i]=1;
        }
        for (int i = 2; i < a; i++) {
            for (int j = 1; j <i; j++) {
                kdd[i][j]=kdd[i-1][j]+kdd[i-1][j-1];
            }
        }
        for (int i = 0; i < a; i++) {
            for (int j = 0; j <= i; j++) {
                System.out.print(kdd[i][j]+"\t");
            }
            System.out.println();
        }
    }
    public static void main(String[] args) {
        yangHui(10);
    }
}//杨辉三角
```

```java
public class Easy {
    public static void main(String[] args) {
        int[] a={1,5,8,6,7,6,45};
        int index=ge1id(a,5);
    }

    private static int ge1id(int[] a, int i) {
        for (int i1 = 0; i1 < a.length; i1++) {
            if(a[i1]==i){
                return i1;
            }
        }
        return -1;
    }
}
```

## 二分法查找

```java
//二分查找前提是有序
public class TwoSearch {
    public static void main(String[] args) {
        int[] a={15,25,36,445,532,645};

        int index=getId(a,15);
        System.out.println(index);
    }

    private static int getId(int[] a, int i) {
        int minIdex=0;
        int maxIndex=a.length-1;
        int centerIndex=(maxIndex+minIdex)/2;
        while (minIdex<=maxIndex) {
            if(i==a[centerIndex]){
                return centerIndex;
            }else if(i>a[centerIndex]){
                minIdex=centerIndex+1;
            }else if(i<a[centerIndex]){
                maxIndex=centerIndex- 1;
            }
            centerIndex=(maxIndex+minIdex)/2;
        }

        return -1;
    }
}
//一直切换中间的对象
```

## 冒泡排序

```java
public class MaoPao {
    public static void main(String[] args) {
        //冒泡排序，两两比较 议论后最大的放在最后
        int[] a={9,5,3,6,4,3};
        a=paiXu(a);
        for (int i:
             a) {
            System.out.println(i);
        }
    }

    private static int[] paiXu(int[] a) {
        int temp=0;
        for (int i = 0; i < a.length; i++) {
            for (int j = 0; j < a.length-1-i; j++) {//因为下面+1，所有小一  避免除法+1
                if (a[j]>a[j+1]){
                    temp=a[j];
                    a[j]=a[j+1];
                    a[j+1]=temp;
                }
            }
        }
        return a;
    }

}//前后比
```

## 选择排序

```java
import java.util.Arrays;

public class XuanZhe {
    public static void main(String[] args) {
        int[] arr={24,69,5,1,78};
        Tuidao(arr);
    }

    private static void Tuidao(int[] arr) {
        for (int index=0;index<arr.length;index++) {
            for (int i = index; i < arr.length; i++) {
                if (arr[index] > arr[i]) {
                    int t = arr[index];
                    arr[index] = arr[i];
                    arr[i] = t;
                }
            }
        }
        System.out.printf( Arrays.toString(arr));
    }
}
//使用第一个和后面的比，找到第一个的位置
```

## 插入排序

//插入有序仍然保存有序

```java
import java.util.Arrays;

public class ChaRu {
    //直接插入排序，从一索引处开始，将后面的元素，插入之前的有序列表中
    public static void main(String[] args) {
        kdd();
    }

    private static void kdd() {
        int[] a={5,9,2,6,4,6,3,44};
        //外层定义轮次
        for (int i = 0; i < a.length; i++) {
            //里层比较
            int j=i;
            while (j>0&&a[j]<a[j-1]){
                int t=a[j];
                a[j]=a[j-1];
                a[j-1]=t;
                j--;
            }
        }
        System.out.println(Arrays.toString(a));
    }
}
```

![image-20200603100416833](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200603100416833.png)

 ## 希尔排序>插入

![image-20200603100741958](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200603100741958.png)

![image-20200603101057894](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200603101057894.png)

```java
import java.util.Arrays;

public class Shel {
    public static void main(String[] args) {
        //对插入的排序的优化
        //直接插入增量位1
        int[] arr={4,89,9,2,5,5};

        Cha(arr);

    }

    private static void Cha(int[] arr) {
        for (int h = arr.length/2; h > 0; h/=2) {
            for (int i = h; i <arr.length ; i++) {
                for (int j = i; j >h-1 ; j-=h) {
                    if(arr[j]<arr[j-h]){
                        int t=arr[j];
                        arr[j]=arr[j-h];
                        arr[j-h]=t;

                    }
                }

            }
        }
        System.out.println(Arrays.toString(arr));
    }
}
//使用言不好 可以使用克鲁特序列
```

int h=1;

while(h<=arr.length/3){h=h*3+1;}



## 快速排序

![image-20200603104218743](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200603104218743.png)

![image-20200603105445151](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200603105445151.png)

## 归并排序

![image-20200603105606501](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200603105606501.png)

![image-20200603105633756](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200603105633756.png)

```java
import java.util.Arrays;

public class GuiBing {
    public static void main(String[] args) {
        int[] arr={9,4,5,7,53,4,85,7,8};
     //   int[] arr={4,5,7,8,1,2,3,6};
        //拆分
        chaiFen(arr,0,arr.length-1);

        //归并
       // guiBing(arr,0,3,arr.length-1);
        System.out.println(Arrays.toString(arr));
    }

    private static void chaiFen(int[] arr, int start, int end) {
        //计算中间索引
        int center=(start+end)/2;
        if(start<end){
            chaiFen(arr,start,center);
            chaiFen(arr,center+1,end);
            guiBing(arr,start,center,end);
        }
    }

    private static void guiBing(int[] arr, int star, int center, int end) {
        //定义一个临时数组
        int[] tempArray=new int[end-star+1];
        //定义左边数组的索引
        int i=star;
        //定义右边数组的索引
        int j=center+1;
        //定义临时数组的索引
        int index=0;
        while(i<=center&&j<=end){
            if(arr[i]<arr[j]){
                tempArray[index++]=arr[i++];
            }else {
                tempArray[index++]=arr[j++];
            }
        }
        //处理剩余元素
        while (i<=center){
            tempArray[index++]=arr[i++];
        }
        while (j<=end){
            tempArray[index++]=arr[j++];
        }
        //System.out.println(Arrays.toString(tempArray));
        //取回
        for (int k = 0; k < tempArray.length; k++) {
            arr[k+star]=tempArray[k];
        }
    }
}

```

## 基数排序

- 分配于收集就可以完成





# Java08

![image-20200603165741067](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200603165741067.png)

## 包装类（基本类型

![image-20200603165858226](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200603165858226.png)

- 在lang包下直接使用
- 自动装箱不是直接new 而是Valuof

```java
import java.util.ArrayList;
import java.util.List;

public class Page {
    /*
    1.什么是包装类
    8种基本数据类型
    每种基本数据类型一一对应



    2.为什么需要
    类的形式提供对象
    字符串与基本数据联系的转换
    缺点
     */
    public static void main(String[] args) {
        List list=new ArrayList();
        list.add(3);//自动装箱/集合的数据类型不能用
        list.add(new Integer(3));//手动装箱
        System.out.println(Integer.MAX_VALUE);
        System.out.println(Integer.toBinaryString(12));
        System.out.println(Integer.toOctalString(12));
        System.out.println(Integer.toHexString(12));
        int i=Integer.parseInt("12364545");//网上注册，输入的都是字符串
        System.out.println(i+1);
        double d=Double.parseDouble("9.156");
        System.out.println(d);
        Integer i1=13;
        int i3=i1;//自动装箱和自动拆箱
        Integer i2=new Integer(5);//手动专向

        int i4=i2.intValue();//手动此项
        System.out.println(i4);
        Integer in1=new Integer(1314159);
        Integer in2=new Integer(1314159);
        Integer in3=5;//自动装箱 不是简单的使用 new Integer();
        Integer in4=5;
        System.out.println(in3.equals(in4));
        System.out.println(in3 == in4);

        System.out.println(in1.equals(in2));//比较的是数据
        System.out.println(in1 == in2);//比较的是地址
    }
    //运行时异常不需要处理，回自动抛出
    //检查异常必须进行异常处理
//可以实现基本类型与数据类型的转变
//

    //缺点
    //包装类需要专用栈内存和对堆内存
    //基本数据类型占用栈内存

/*
 public boolean equals(Object obj) {
        if (obj instanceof Integer) {
            return value == ((Integer)obj).intValue();
        }
        return false;
    }
 */
/*
public static Integer valueOf(int i) {
        if (i >= IntegerCache.low && i <= IntegerCache.high)
            return IntegerCache.cache[i + (-IntegerCache.low)];//若在-128到127 直接返回
        return new Integer(i);//如果在外需要创建对象
    }
 */
    /*
     private final int value;

     public Integer(int value) {
        this.value = value;
    }
     */
    /*
     static {
            // high value may be configured by property
            int h = 127;
            String integerCacheHighPropValue =
                sun.misc.VM.getSavedProperty("java.lang.Integer.IntegerCache.high");
            if (integerCacheHighPropValue != null) {
                try {
                    int i = parseInt(integerCacheHighPropValue);
                    i = Math.max(i, 127);
                    // Maximum array size is Integer.MAX_VALUE
                    h = Math.min(i, Integer.MAX_VALUE - (-low) -1);
                } catch( NumberFormatException nfe) {
                    // If the property cannot be parsed into an int, ignore it.
                }
            }
            high = h;

            cache = new Integer[(high - low) + 1];
            int j = low;
            for(int k = 0; k < cache.length; k++)
                cache[k] = new Integer(j++);

            // range [-128, 127] must be interned (JLS7 5.1.7)
            assert IntegerCache.high >= 127;
        }
     */
}
```

## 字符串的相关类

```java
import java.util.Arrays;
/*
总结
length
toUperCase
toLowerCase
charAt
indexOf
concat
toCharArray()
substring
replace
 */
public class StringTest {
    public static void main(String[] args) {
        //创建字符串对象
        String s1="我喜欢你康丹丹LDD Dkdd    ";//不可变的，需要创建，改变引用
        String s2=new String("嗯嗯");
        //长度 大小写转换 判断其实字符串 结束 中间
        System.out.println(s1.length());//字符的个数，不是直接的个数
        System.out.println(s1.toUpperCase());
        System.out.println(s1.toLowerCase());//类型是不可变，他重新创建了应该空间
        System.out.println(s1.startsWith("我"));//开始
        System.out.println(s1.endsWith("d"));//结尾
        System.out.println(s1.contains("康丹丹"));//包含
        System.out.println(s1.charAt(1));
        System.out.println(s1.substring(2, 4));
        System.out.println(s1.substring(2));
        System.out.println(s1.indexOf("康"));
        System.out.println(s1.concat("赵朝进"));//拼接都是形成新的字符串
        System.out.println(s1.replace("康丹丹", "康丹"));
        System.out.println(s1.isEmpty());//判断是否为空  str="";//指向堆 str=null;//狗jb不是
        System.out.println(s1.replaceAll("D", "a"));
        System.out.println(s1.replace("D", "a"));
        char[] a=s1.toCharArray();
        System.out.println(s1.trim()+"hello");//去掉两端的空格
        int ai[]=new int[a.length];
        for (int i = 0; i < a.length; i++) {
            ai[i]=a[i];
        }
        System.out.println(Arrays.toString(ai));
    }
}

```



![image-20200604123209292](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200604123209292.png)

==比较栈内存的内容

.equals值

![image-20200605081907716](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200605081907716.png)

```java
package com.kangsdan;

public class StringBuf {

    /*
    private final char value[];//底层是字符数组
    public String() {
        this.value = "".value;
    }
    //字符串在常量池中，将给堆内存中的value属性

     public String(String original) {
        this.value = original.value;
        this.hash = original.hash;
    }
     */

    /*public boolean equals(Object anObject) {
           if (this == anObject) {
                return true;
            }//引用相同，内容相同
            if (anObject instanceof String) {
                String anotherString = (String)anObject;//字符长度
                int n = value.length;//原始长度
                if (n == anotherString.value.length) {
                //获取底层的数组
                    char v1[] = value;
                    //同上
                    char v2[] = anotherString.value;
                    int i = 0;
                    while (n-- != 0) {
                        if (v1[i] != v2[i])
                            return false;
                        i++;
                    }

                    return true;
                }
            }
            长度不相同，直接返回错误
            return false;
        }
     */
    /*
    public String concat(String str) {
        int otherLen = str.length();
        if (otherLen == 0) {
            return this;
        }
        //获取原来的长度
        int len = value.length;
        char buf[] = Arrays.copyOf(value, len + otherLen);//在常量池中有新的创建
        str.getChars(buf, len);
        //追加的字符串
        return new String(buf, true);
    }
     */
    public static void main(String[] args) {
        String string=new String();
        String string1=new String("康丹丹赵朝进");
        System.out.println(string1.length());
        System.out.println(string1.isEmpty());
        System.out.println(string1.charAt(3));//value[3]
        String s=new String("康丹丹赵朝进");//常量池中就只有一次
        System.out.println(s == string1);//堆内存重新创建
        System.out.println(s.equals(string1));//常量池中就只有一次
        String s2="康丹丹";
        s2=s2.concat("abc");
        System.out.println(s2);
    }


}

```

```java
/*
 public int compareTo(String anotherString) {
        int len1 = value.length;
        int len2 = anotherString.value.length;
        int lim = Math.min(len1, len2);
        char v1[] = value;
        char v2[] = anotherString.value;

        int k = 0;
        while (k < lim) {
            char c1 = v1[k];
            char c2 = v2[k];
            if (c1 != c2) {
                return c1 - c2;
            }
            k++;
        }
        return len1 - len2;
    }
 */
public class TestString {
    public static void main(String[] args) {
       // "".equals()判断对象的类容是否相同
        String s1="康丹丹";
        String s2="康丹丹";
        String s4="康丹丹A";
        String s5="康丹丹a";
        String s6="康丹丹AK";

        String s3=new String("康丹丹");
        System.out.println(s1.equals(s2));
        System.out.println(s1 == s2);
        System.out.println(s1.equals(s3));
        System.out.println(s1 == s3);
        //"".compareTo()比较对象大小是否相同
        System.out.println(s1.compareTo(s4));
        System.out.println(s4.compareTo(s5));
        System.out.println(s5.compareTo(s6));

        //字符串数组之间的转换
        char[] a=s6.toCharArray();
        /*
        public char[] toCharArray() {
        // Cannot use Arrays.copyOf because of class initialization order issues
        char result[] = new char[value.length];
        System.arraycopy(value, 0, result, 0, value.length);
        return result;
        }
         */
        String s = new String(a);
        String ss=new String(a,1,2);
        //引入StringBuffer StringBuilder
        String ss1=new String("abxc");
        ss1.concat("1");
        ss1.concat("2");//每次调用都会生成应该中间的字符串吗，会浪费空间，效率低下
        //String被设计为不可变字符串
        //要直接追加，需要考虑数组长度不够的问题
        System.out.println(ss1);
    }
}
```

# Java 09

## StringBuffer StringBuilder

```java
package com.kangsdan;

public class TestStringBuilder {
    //底层都是数组
    public static void main(String[] args) {
/*
 AbstractStringBuilder(int capacity) {
        value = new char[capacity];//当上面是数值的时候
    }
 */
        /*
        public StringBuilder(String str) {
        super(str.length() + 16);
        append(str);
    }
         */
       //创建 StringBuilder
        StringBuilder stringBuilder = new StringBuilder("1223");//直接数值不一样
        stringBuilder.append(1223);

        stringBuilder.append("kdd");
        stringBuilder.append("1234567891234567");
        stringBuilder.append("123");
        System.out.println(stringBuilder);
        String ss= String.valueOf(stringBuilder);
        /*
        public static String valueOf(Object obj) {
            return (obj == null) ? "null" : obj.toString();
        }
         */
        /*
        public String toString() {
        // Create a copy, don't share the array
            return new String(value, 0, count);
         }
         */
        String ss1=stringBuilder.toString();
        System.out.println(ss == ss1);
        System.out.println(ss.equals(ss1));
        //追加
        stringBuilder.insert(3,3.15);
        System.out.println(stringBuilder);


        //删除

        stringBuilder.delete(3,7);
        System.out.println(stringBuilder);
        //修改
        stringBuilder.setCharAt(1,'1');
        stringBuilder.replace(1,3,"adadadd");
        System.out.println(stringBuilder);

        //反转
        System.out.println(stringBuilder.reverse());


        //转换
        //toString();
    }
}

```

```java
package com.kangsdan;
/*
public StringBuilder append(String str) {
        super.append(str);
        return this;
    }/*
 */
/*
public AbstractStringBuilder append(String str) {
        if (str == null)
            return appendNull();
        int len = str.length();
        //扩容
        ensureCapacityInternal(count + len);
        str.getChars(0, len, value, count);
        count += len;
        return this;
    }
 */
/*
public void getChars(int srcBegin, int srcEnd, char dst[], int dstBegin) {
        if (srcBegin < 0) {
            throw new StringIndexOutOfBoundsException(srcBegin);
        }
        if (srcEnd > value.length) {
            throw new StringIndexOutOfBoundsException(srcEnd);
        }
        if (srcBegin > srcEnd) {
            throw new StringIndexOutOfBoundsException(srcEnd - srcBegin);
        }
        System.arraycopy(value, srcBegin, dst, dstBegin, srcEnd - srcBegin);//直接在后面追加1的内容
    }
 */
public class TestStringBuffer {
    public static void main(String[] args) {
        StringBuilder stringBuilder=new StringBuilder();
        System.out.println(stringBuilder.length());
        System.out.println(stringBuilder.capacity());
        stringBuilder.append("1212");
        System.out.println(stringBuilder.length());
        System.out.println(stringBuilder.capacity());
        stringBuilder.append("12124556465465");
        System.out.println(stringBuilder.length());
        System.out.println(stringBuilder.capacity());
    }
}/*
 public String toString() {
        // Create a copy, don't share the array
        return new String(value, 0, count);
    }*/

```

- 底层相同
- 先有StringBuffer  再有StringBulider
- StringBuffer线程安全、性能低下（有锁
- StringBuilder线程不安全  性能高（无锁
- java性能低下，和c语言向比较（每次运行class需要解释为机器码

## Javap -c test

```java
public class T1 {
    public static void main(String[] args) {
        String a="5454"+"sda";//字面常量编译的时候会优化，直接编译成为字符串
        String b=a+"sdd";//底层还是才用StringBuilder
        //System.out.println(b);
        for (int i = 0; i < 100; i++) {
            a+=i;//创建了多个StringBuilder
        }
        System.out.println(a);
        StringBuilder stringBuilder=new StringBuilder();
        for (int i = 0; i < 100; i++) {
            stringBuilder.append(i);//始终只有一个
        }
        System.out.println(stringBuilder.toString());
        System.out.println(stringBuilder);
    }
}
```

```java
public class T1 {
    public static void main(String[] args) {
       StringBuilder a=new StringBuilder("A");
       StringBuilder b=new StringBuilder("B");
       mb_oper(a,b);
        System.out.println(a + "." + b);
    }

    private static void mb_oper(StringBuilder a, StringBuilder b) {
        a.append(b);
        b=a;
    }
}
```

![image-20200605114423844](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200605114423844.png)

```java
import java.util.Scanner;

public class Test01 {
    public static void main(String[] args) {
        Scanner scanner=new Scanner(System.in);
        String a=scanner.nextLine();
        if(a.length()<6){
            System.out.println("长度小于6");
            return;
        }
        char[] b=a.toCharArray();
        for (int i = 0; i < b.length; i++) {
            if(b[i]>'0'&&b[i]<'9'||b[i]==' '){
                System.out.println("包含了错误类型");
                return;
            }
        }
        System.out.println(a);
        scanner.close();
    }
}
```

## 时间处理的相关类

![image-20200605115430321](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200605115430321.png)

## 日期的date

- util

```java
import java.util.Date;

public class DateTest {
    //获取当前下单的时间，存到数据库
    public static void main(String[] args) {
        //获取当前的时间
        Date date=new Date();//1970-1-1 8:00:00   毫秒
        //public Date() {
        //        this(System.currentTimeMillis());
        //    }
        /*
        private transient long fastTime;
         */
        //输出下单的时间
        System.out.println(date.toString());
        System.out.println(date.toLocaleString());
        //认识过时的
        System.out.println(date.getYear());//1900+118
        System.out.println(date.getDay());//周几

        //没有过时的方法
        long da=date.getTime();//返回了毫秒数
        System.out.println(da);
    }
}

```

- sql

```java
import java.sql.Date;

public class Datet {
    /*
    java.util.Date   YYYYMMDDHHMMSS
    java.sql.Date   YYYYMMDD
    java.sql.Time   HHMMSS
    java.sql.Tamp   YYYYMMDDHHMMSS
    都与数据库的操作有管
     */
    public static void main(String[] args) {
        //创建  sql没有无参数的构造
        Date now =new Date(System.currentTimeMillis());
        System.out.println(now);
        //方法  util没有方法
        Date date2=Date.valueOf("1999-12-23");//直接
        System.out.println(date2);
        //sql->date
        Date date=new Date(System.currentTimeMillis());
        System.out.println(date);
        java.util.Date up=date;
        java.util.Date up1=date2;//字类到父类
        //根据多态的原理，父类引用调用方法，如果字类重写，调用子类的方法
        System.out.println(up.toString());
        java.util.Date ud=new java.util.Date(date.getTime());//返回毫秒数
        System.out.println(ud);
        System.out.println(up1);
        //util->sql
        java.util.Date ud1=new java.util.Date();
        System.out.println(ud1);
        Date date1=new Date(ud1.getTime());
        System.out.println(date1);
    }
}

```

- Date Formate

```java
import java.util.Date;
import java.text.DateFormat;
import java.text.ParseException;
import java.text.SimpleDateFormat;

public class Simp {
    /*
    需求1：网页注册，网页所有的内容都是字符串 日期<->字符串
    需求2：后台有日期，注册成功后再网页上的日期
     */
    public static void main(String[] args) throws ParseException {
        //方法一  sql
//        Date date = Date.valueOf("1923-12-6");//太弱
//        System.out.println(date.toString());
        //方法
        int a=Integer.parseInt("23");
        //创建有管DateFormate
        DateFormat dateFormat=new SimpleDateFormat("yyyy-MM-dd");//mm代表分钟
        String av="1999-1-16";
        //字符串到日期。

        java.util.Date date1=dateFormat.parse(av);
        System.out.println(date1.toLocaleString());
//日期到字符串
        DateFormat dateFormat1=new SimpleDateFormat("yyyy年MM月dd日hh时mm分ss秒");
        String str =dateFormat1.format(date1);
        System.out.println(str);
    }
}

```

- Calendar淘汰了Date

```java
import java.util.Calendar;
import java.util.GregorianCalendar;

public class DateKING {
    public static void main(String[] args) {
        Calendar calendar=new GregorianCalendar();
        System.out.println(calendar.get(Calendar.YEAR));
        System.out.println(calendar.get(Calendar.MONTH));
        System.out.println(calendar.get(Calendar.DATE));
        System.out.println(calendar.get(Calendar.DAY_OF_WEEK));//周日是第一天
        calendar.set(Calendar.DATE,1);
        for (int i = 0; i < 35; i++) {
            calendar.add(Calendar.DATE,1);
            System.out.println(calendar.get(Calendar.DATE));
        }
        System.out.println(calendar.getActualMaximum(Calendar.DATE));
    }
}
```

## 枚举

```java
public class Enums {
    private String name;
    private String sex;
    private int age;

    @Override
    public String toString() {
        return "Enums{" +
                "name='" + name + '\'' +
                ", sex='" + sex + '\'' +
                ", age=" + age +
                '}';
    }

    public static void main(String[] args) {
        Enums enums=new Enums();
        enums.age=11;
        enums.name="张三丰";
        enums.sex="男";
        System.out.println(enums.toString());
    }
}

```

- win1.5提供

```java
public enum Season {
    春,夏,秋,冬
}

```

```java
public class TestSeason {


    public static void main(String[] args) {
        Season season=Season.冬;
        switch (season){
            case 冬:
                System.out.println("cloude");
                break;
            case 夏:
                System.out.println("热");
                break;
            case 春:
                System.out.println("安逸");
                break;
            case 秋:
                System.out.println("砍头");
        }
    }
}/*

*/

```

![image-20200605191244823](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200605191244823.png)

## swith int short string char enum

 ```java
import java.util.Random;

public class TestMatch {
    public static void main(String[] args) {

        System.out.println(Math.abs(-5));
        System.out.println(Math.round(3.5));//四舍五入
        System.out.println(Math.ceil(3.5));//取大
        System.out.println(Math.floor(3.5));//取小

        System.out.println(Math.max(20, 30));//最大值
        System.out.println(Math.min(15, 2));//最小
        System.out.println(Math.pow(3, 3));//平方
        System.out.println(Math.random());//0.0-1
        System.out.println(Math.sqrt(4));//开跟
        Random r=new Random(System.currentTimeMillis());
        for (int i = 0; i < 10; i++) {
            System.out.println(r.nextInt(10));
        }

    }
}


import java.util.Random;

public class TestMatch {
    public static void main(String[] args) {

        System.out.println(Math.abs(-5));
        System.out.println(Math.round(3.5));//四舍五入
        System.out.println(Math.ceil(3.5));//取大
        System.out.println(Math.floor(3.5));//取小

        System.out.println(Math.max(20, 30));//最大值
        System.out.println(Math.min(15, 2));//最小
        System.out.println(Math.pow(3, 3));//平方
        System.out.println(Math.random());//0.0-1
        System.out.println(Math.sqrt(4));//开跟
        Random r=new Random(System.currentTimeMillis());
        System.out.println("sda");
        /*
        [10,20]-->[10,21)-->10+[0,11)
         */
        /*
        int()强准
         */
        for (int i = 0; i < 10; i++) {
            System.out.println(r.nextInt(100));
        }

    }
}
 ```

## File

![image-20200605194751323](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200605194751323.png)

```java
import java.io.File;
import java.text.DateFormat;
import java.text.SimpleDateFormat;
import java.util.Arrays;
import java.util.Date;

public class TestFile01 {
    /*
        文件和目录的抽象表示形式
        获取文件夹的属性
        创建和删除文件和文件夹
        不能访问文件的内容，需要Io流来创建
         */
    public static void main(String[] args) {
        //创建，指向文件或者文件夹
        File file=new File("C:\\Users\\1\\Desktop\\61");//
        //模拟dir
        System.out.println(file.getName());
        System.out.println(file.exists());
        System.out.println(file.length());//文件类容的字节
        System.out.println(file.getAbsoluteFile());
        System.out.println(file.getPath());
        System.out.println(file.canWrite());//可写
        System.out.println(file.isHidden());//隐藏
        String[] files=file.list();//前提是指向目录的,返回文件文件夹名称
        File[] files1=file.listFiles();
        System.out.println(Arrays.toString(files));
        System.out.println(Arrays.toString(files1));
        //时间
        Date date=new Date(file.lastModified());
        System.out.println(date.toLocaleString());

        //类型
        for (int i = 0; i < files1.length; i++) {
            date=new Date(files1[i].lastModified());
            System.out.print(date.toLocaleString()+"\t");
            if(files1[i].isDirectory()){
                System.out.println("DIR+\t");
            }

            else {
                System.out.println(files1[i].getName());
            }
        }


        //长度

        //名称
    }
}
```

- 创建

```java
import java.io.File;
import java.io.IOException;
/*
指向一个文件 或者一个目录的
创建文件，创建文件夹
 */
public class Make {
    /*
    文件的创建和删除
     */
    public static void main(String[] args) {
        //创建
        File file=new File("C:\\Users\\1\\Desktop\\61\\hello.txt");
        //存在删除
        if(file.exists()){
            file.delete();
        }
        //不存在创建
        else {
            try {
                //判断上级文件夹是否存在
                //创建文件
                File dir=file.getParentFile();
                file.createNewFile();
                if(!dir.exists()){
                    //创建文件夹
                    dir.mkdirs();
                }
            } catch (IOException e) {
                e.printStackTrace();
            }
        }
    }
}

```

![image-20200605205810457](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200605205810457.png)


# Java10

## 集合容器

![image-20200606154541590](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200606154541590.png)

![image-20200606154620557](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200606154620557.png)

- 相同的结构的整合到一起的时候就可以考虑到集合

## 集合与数组

- 相同点

都可以放多个元素，对外当一个整体。

- 不同点（缺点

数组的长度的

动态扩容，产生了新的数组，

数组需要开辟连续的空间   添加删除的效率低下

没有办法保存映射关系

缺少封装，操作比较繁琐

![image-20200606155813620](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200606155813620.png)

ArrayList与数组有关系，其它的完全不同

![image-20200606160008003](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200606160008003.png)

## Collection 接口存储一组不唯一 无序对象



###  List 接口存储一组不唯一，有序的对象

- ArryList

![image-20200606161107682](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200606161107682.png)

```java
package com.kangsdan.List;

import java.util.ArrayList;
import java.util.Arrays;
import java.util.Iterator;

/*
存储多个分数
分数不唯一，不唯一   有先后顺序
 */
/*
常用方法
添加单个对象
添加集合
元素个数size
元素的获取get

list.Itreator   list数据交给迭代器
 */
public class TestArrayList {
    public static void main(String[] args) {
        //创建一个集合对象来存储多个分数
        ArrayList list = new ArrayList();//初始分配分配空间，不关注
        ArrayList list1 = new ArrayList();

        //使用这个对象存储多个分数
        list1.add(100);
        list1.add(101);
        list1.add(102);

        list.addAll(list1);
        list.addAll(3, list1);
        list.add(3);//集合中只能放对象不能放基本类型
        list.add(341);
        list.add(34);
        list.add(3);
        list.add(3);
        list.add(3);
        list.add(3, 88);
        //输出集合中所有的分数
//        System.out.println(list.size());//元素的个数，不是表示分配了多少个空间
//        System.out.println(list);
//        System.out.println(list.get(3));
        //普通for
        for (int i = 0; i < list.size(); i++) {
            System.out.print(list.get(i) + ",");//是object需要强转int
        }
        System.out.println("two");
        //增强for
        for (Object i : list
        ) {
            System.out.print(i + ",");
        }
        //Itreator
        System.out.println("three");
        Iterator iterator = list.iterator();
        while (iterator.hasNext()) {//true ,false
            int el = (int) iterator.next();//就算指针移动一次
            System.out.print(el+",");
        }
    }
}

```



```java
package com.kangsdan.List;

import java.util.ArrayList;
import java.util.Iterator;

public class TestArryList2 {
    /*
    缺点，取出元素需要强制转换（繁琐
    添加的元素数据类型可以不同（不安全

    泛型
    安全感
    简单
     */
    public static void main(String[] args) {
        ArrayList<Integer> arrayList=new ArrayList<Integer>();
        arrayList.add(3);
        arrayList.add(4);
        arrayList.add(5);
        arrayList.add(6);
        arrayList.add(7);
        for (int i = 0; i < arrayList.size(); i++) {
            int a=arrayList.get(i);
            System.out.print(a+",");
        }
        System.out.println();
        Iterator<Integer> iterator = arrayList.iterator();
        while (iterator.hasNext()){
            int n=iterator.next();
            System.out.print(n+",");
        }
    }

}

```

```java
package com.kangsdan.List;

import java.text.DateFormat;
import java.text.ParseException;
import java.text.SimpleDateFormat;
import java.util.ArrayList;
import java.util.Date;

public class TestArryList3 {
    public static void main(String[] args) throws ParseException {
        ArrayList list = new ArrayList();
        list.add(3);//集合中只能放对象不能放基本类型
        list.add(341);
        list.add(34);
        list.add(34);
        list.add(3);
        list.add(43);
        list.set(1,44);
        list.remove(1);
        list.remove(new Integer(88));
        //list.removeAll();
        System.out.println(list);
        System.out.println(list.indexOf(new Integer(34)));
        list.clear();
        System.out.println(list.contains(new Integer(34)));
    }

}

```

```java
package com.kangsdan.List;

import java.util.ArrayList;

/*
public class ArrayList<E> extends AbstractList implements List<E>
transient Object[] elementData;//底层是数组，空间没有分配
private static final Object[] DEFAULTCAPACITY_EMPTY_ELEMENTDATA = {};
 private int size;

public ArrayList() {
        this.elementData = DEFAULTCAPACITY_EMPTY_ELEMENTDATA;
    }无参数是0个空间

     public ArrayList(int initialCapacity) {
        if (initialCapacity > 0) {
            this.elementData = new Object[initialCapacity];
        }{





 private static int calculateCapacity(Object[] elementData, int minCapacity) {
        if (elementData == DEFAULTCAPACITY_EMPTY_ELEMENTDATA) {
            return Math.max(DEFAULT_CAPACITY, minCapacity);
        }
        return minCapacity;
    }


    private void ensureCapacityInternal(int minCapacity) {
        ensureExplicitCapacity(calculateCapacity(elementData, minCapacity));
    }

     private void ensureExplicitCapacity(int minCapacity) {

        if (minCapacity - elementData.length > 0)//如果最小大于地城就扩容
            grow(minCapacity);
    }



     private void grow(int minCapacity) {
        // overflow-conscious code
        int oldCapacity = elementData.length;//就容量
        int newCapacity = oldCapacity + (oldCapacity >> 1);//10+5每次扩容1/2
       //如果还是
        if (newCapacity - minCapacity < 0)
            newCapacity = minCapacity;
       //老数组行容量，新创建一个更大容量的数据
        elementData = Arrays.copyOf(elementData, newCapacity);
    }

 */
public class TestArryList {
    public static void main(String[] args) {
        ArrayList arrayList=new ArrayList(3);
        arrayList.add(3);
        /*
         public boolean add(E e) {
        ensureCapacityInternal(size + 1);  // Increments modCount!!
        elementData[size++] = e;//夹到集合的最后数量加油  返回size的时候终结就是这个
        return true;
    }
         */
        arrayList.get(0);
        /*
         public E get(int index) {
        rangeCheck(index);

        return elementData(index);
    }
         */
        System.out.println(arrayList.toString());
        /*
           public String toString() {
        Iterator<E> it = iterator();
        if (! it.hasNext())
            return "[]";

        StringBuilder sb = new StringBuilder();
        sb.append('[');
        for (;;) {
            E e = it.next();
            sb.append(e == this ? "(this Collection)" : e);
            if (! it.hasNext())
                return sb.append(']').toString();
            sb.append(',').append(' ');
        }
    }

}
         */
        arrayList.iterator();
        /*
         public Iterator<E> iterator() {
        return new Itr();//一个内部类，实现了接口
    }
    private class Itr implements Iterator<E> {
        int cursor;       // 当前位置
        int lastRet = -1; // 前一个位置
        int expectedModCount = modCount;

        Itr() {}

        public boolean hasNext() {
            return cursor != size;//判断是否有元素  广百哦是否指向最后一个元素的后一个
        }

        @SuppressWarnings("unchecked")
        public E next() {

            int i = cursor; //i=0

            cursor = i + 1;//cursor=1;
            return (E) elementData[lastRet = i];
        }


         */

    }


}

```



- Lineklist

![image-20200606161148253](C:\Users\1\AppData\Roaming\Typora\typora-user-images\image-20200606161148253.png)



### set 接口存储一组唯一的，无序的对象



## Map接口存储一组键值对象，提供key到value的映射

- key唯一无序
- valu不唯一无序

# Java 11

