# 范冬冬ch0学习笔记

#### 问题1：如何在Mac os系统里运行python3,因为系统自带python2.7,有人说Mac上会出现python3不兼容现象。

* 尝试：首先搜索“如何在mac os系统上安装python3”,结果发现自己已经装了IDLE。
  ```
   then-搜索如何在terminal里运行python3：可直接在Terminal里面输入'python3',回车即可。
   在python3交互环境下，如何退出，有三种方式：exit();quit();ctl+d.
  ```

#### 问题2：terminal用python3运行ex1.py

```
   输入： pathon3 ex1.py
   返回：-bash: pathon3: command not found
```

* 尝试1、检查：python写错为pathon
* 尝试2、输入：python3 ex1.py
  ```
    返回：No such file ex1.py
  ```
* 尝试3、继续检查：发现所在文件夹不对
* 尝试4、切换至正确文件夹。

  ```
    输入：python3 ex1.py
    返回： File "ex1.py", line 1
          print "Hello World!"
          ^
          SyntaxError: Missing parentheses in call to 'print'

    意思是在执行print命令时，少了圆括号，但是我不明白是哪里少了，于是上网搜索，结果为：In Python 3 you need to add parentheses around the value to be printed:print("Hello world") ，所以我知道了，应该在print 后面加上圆括号.
    解决方案链接 [What does “SyntaxError: Missing parentheses in call to ‘print’” mean in Python? - Stack Overflow](http://stackoverflow.com/questions/25445439/what-does-syntaxerror-missing-parentheses-in-call-to-print-mean-in-python/)，同时这里有很多关于python的问题，已将该网站收藏。
  ```

* 尝试5、加上圆括号后。

  ```
    输入：python3 ex1.py
    返回：SyntaxError: Missing parentheses in call to 'print'
         再检查：可能是圆括号没有紧挨着print，中间出现了一个空格，删掉空格后，输出结果为
     File "ex1.py", line 1
     print（"Hello World!"）
     ^
     SyntaxError: invalid character in identifier

    继续检查：圆括号可能是在中文输入模式下输入的，改正后尝试。

    输入: python3 ex1.py
    返回：Hello World!
         Hello Again
         I like typing this.
         This is fun.
         Yay! Printing.
         I'd much rather you 'not'.
         I "said" do not touch this.
      终于正确。
  ```

* 尝试6、在解决这个问题的时候，同时学习了一下如何在IDLE里写基本程序 [Python学习笔记（0） - ﹏猴子请来的救兵 - 博客园](http://www.cnblogs.com/yyhh/p/4202829.html)， [17个新手常见Python运行时错误 - 开源中国社区](http://www.oschina.net/question/89964_62779/) ，[https://github.com/OpenMindClub/learn-python/blob/master/101%20-%20Python入门.ipynb，真是有意思。](https://github.com/OpenMindClub/learn-python/blob/master/101%20-%20Python入门.ipynb，真是有意思。)

## 



