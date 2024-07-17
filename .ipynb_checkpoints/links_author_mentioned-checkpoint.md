# 作者提到的必须要看的文章或者文档

## 一 阅读的内容

### 1.1 Must have

Python官方文档：
- [ ] [The Python Tutorial](https://docs.python.org/3/tutorial/index.html)
- [ ] [Standard Libraries](https://docs.python.org/3/library/index.html)      
- [ ] [Language References](https://docs.python.org/3/reference/index.html)
- [ ] Python 中有一个概念叫 PEP，[Python Enhancement Proposals](https://www.python.org/dev/peps/pep-0008/)，必须找时间阅读，反复阅读，牢记于心。
--- 

方法论：

- [ ] 作为一个有素养的自学者，有一篇文章必须精读：[How To Ask Questions The Smart Way](https://github.com/selfteaching/How-To-Ask-Questions-The-Smart-Way)

---

概念： 

- [ ] https://en.wikipedia.org/wiki/Context-free_grammar
- [ ] https://en.wikipedia.org/wiki/Backus-Naur_form
- [ ] https://en.wikipedia.org/wiki/Glob_(programming)
- [ ] https://en.wikipedia.org/wiki/Wildcard_character

### 1.2 Should have

Python官方文档：
- [ ] [文档规范](https://devguide.python.org/documenting/)
- [ ] [doctest —— Test interactive Python examples](https://docs.python.org/3/library/doctest.html)
- [ ] [unittest —— Unit testing framework](https://docs.python.org/3/library/unittest.html)

---

方法论：

- [X] [MoSCoW Method](https://en.wikipedia.org/wiki/MoSCoW_method) 
- [ ] https://www.lifehack.org/articles/technology/20-tips-use-google-search-efficiently.html



### 1.3 Could have

- [ ] [Read the Docs](https://readthedocs.org)
- [X] [What exactly can you do with Python? ](https://medium.freecodecamp.org/what-can-you-do-with-python-the-3-main-applications-518db9a68a78)
- [ ] [Iterables vs. Iterators vs. Generators](https://nvie.com/posts/iterators-vs-generators/)


顺带给你看个 Wikipedia 上的链接列表，在编程领域里，有无数可以借鉴到生活中的哲学、方法论：
> - [ ] [If it ain't broke, don't fix it](https://en.wikipedia.org/wiki/If_it_ain%27t_broke,_don%27t_fix_it)
> - [ ] [KISS principle](https://en.wikipedia.org/wiki/KISS_principle)
> - [ ] [Don't repeat yourself](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)
> - [ ] [Feature creep](https://en.wikipedia.org/wiki/Feature_creep)
> - [ ] [List of software development philosophies](https://en.wikipedia.org/wiki/List_of_software_development_philosophies)
> - [ ] [Minimum viable product](https://en.wikipedia.org/wiki/Minimum_viable_product)
> - [ ] [MoSCoW method](https://en.wikipedia.org/wiki/MoSCoW_method)
> - [ ] [Overengineering](https://en.wikipedia.org/wiki/Overengineering)
> - [ ] [Worse is better](https://en.wikipedia.org/wiki/Worse_is_better)
> - [ ] [S.O.L.I.D.](https://en.wikipedia.org/wiki/SOLID)
> - [ ] [Unix philosophy](https://en.wikipedia.org/wiki/Unix_philosophy)


--- 

乔治·布尔  

- [ ] [THE MATHEMATICAL ANALYSIS OF LOGIC](http://www.gutenberg.org/ebooks/36884) 
- [ ] [AN INVESTIGATION OF THE LAWS OF THOUGHT](http://www.gutenberg.org/ebooks/15114)
- [ ] [A TREATISE ON DIFFERENTIAL EQUATIONS](https://archive.org/details/atreatiseondiff06boolgoog/page/n7)

--- 

香农·布朗

- [ ] [A SYMBOLIC ANALYSIS OF RELAY AND SWITCHING CIRCUITS](https://www.cs.virginia.edu/~evans/greatworks/shannon38.pdf)
- [ ] [The Logician and the Engineer: How George Boole and Claude Shannon Created the Information Age](https://www.amazon.com/gp/product/B0091XBUTM/ref=dbs_a_def_rwt_hsch_vapi_tkin_p1_i4)


### 1.4 Won't have

***先看完官方文档，避免先看各种二手教程***

---

## 二 要点

牢记且遵守这个原则, ***第一查询对象只能是官方文档***。用 Google 查询官方文档：

> `<queries> site:python.org`

有时甚至会指定在哪个目录里搜索：
    
> `bytes site:python.org/3/library`，你试试这个连接：[bytes site:python.org/3/library](https://www.google.com/search?q=byte+site%3Apython.org%2F3%2Flibrary)

这个原则对任何语言都适用。将来你在学习任何新软件包（库）、语言更新后的新特性、甚至另外一个新语言的时候，都要这么做。所谓的超强自学能力，基本上就是由一些类似这样的小习惯和另外一些特别基础的方法构成的强大能力。

---

## 三 String、操作符和文件的简单总结


![](../images/string-concepts.png)

--- 

Python 针对数字常用的操作符和内建函数，按照**优先级**从低到高排列：

|名称  | 操作               | 结果                                                       | 官方文档链接                                           |
| --- | ----------------- | ------------------------------------------------------------| ------------------------------------------------------------ |
| 加  | `1 + 2`           | 3                                          |                                                              |
| 减  | `2 - 1`           | 1                                    |                                                              |
| 乘  | `3 * 5`           | 15                                       |                                                              |
| 除  | `6 / 2`           | 3.0                                      |                                                              |
| 商  | `7 // 3`          | 2                              |                                                              |
| 余  | `7 % 3`           | 1                              |                                                              |
| 负  | `-6`              | -6                             |                                                              |
| 正  | `+6`              | 6                              |                                                              |
| 绝对值 | `abs(-1)`         | 1                           | [`abs()`](https://docs.python.org/3/library/functions.html#abs) |
| 转换为整数| `int(3.14)`       | 3                        | [`int()`](https://docs.python.org/3/library/functions.html#int) |
| 转换为浮点数 | `float(3)`        | 3.0                   | [`float()`](https://docs.python.org/3/library/functions.html#float) |
| 商余 | `divmod(7, 3)`    | 2, 1                         | [`divmod()`](https://docs.python.org/3/library/functions.html#divmod) |
| 幂 | `pow(2, 10)`      | 1024                          | [`pow()`](https://docs.python.org/3/library/functions.html#pow) |
| 幂 | `3 ** 2`          | 9                             |                                                              |

---

![](../images/list-concepts.png)

---

文本文件的基本操作：

> * 打开文件，直接用内建函数，`open()`，基本模式有 `r` 和 `w`；
> * 删除文件，得调用 `os` 模块，使用 `os.remove()`，删除文件前最好确认文件确实存在……
> * 读写文件分别有 `file.read()`、`file.write()`、`file.readline()`、`file.readlines()`、`file.writelines()`；
> * 可以用 `with` 把相关操作都放入同一个语句块……

---

