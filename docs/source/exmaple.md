[toc]



## 任务一 Module-level dependency analysis （By snakefood）



### 实验步骤



#### Linux Ubuntu

- 安装 snakefood

  `` pip install snakefood``

- 生成 依赖关系文件 （1.deps）

![ub_sna_1](E:\Desktop\学校\三上\软件体系结构\dot\ub_sna_1.png)

- 生成 dot文件 （1.dot）

![ub_sna_2](E:\Desktop\学校\三上\软件体系结构\dot\ub_sna_2.png)

- 在线网站生成图片



#### Windows

- 安装 snakefood

`` pip2 install snakefood``   ~~我的PC python2，3兼容~~

- 生成 依赖关系文件 （1.deps）

![win_sna_1](E:\Desktop\学校\三上\软件体系结构\dot\win_sna_1.jpg)



- 生成 dot文件 （1.dot）

![win_sna_2](E:\Desktop\学校\三上\软件体系结构\dot\win_sna_2.jpg)

- 在线网站生成图片



### 实验结果

- 1.deps

  ```
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'UseSqlite.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'UseSqlite.py'), ('C:\\Python27\\lib', 'sqlite3'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'WordFreq.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'WordFreq.py'), ('C:\\Python27\\lib', 'string.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'WordFreq.py'), ('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'wordfreqCMD.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'difficulty.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'difficulty.py'), ('C:\\Python27\\lib', 'math'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'difficulty.py'), ('C:\\Python27\\lib', 'pickle.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'difficulty.py'), ('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'wordfreqCMD.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'main.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'pickle_idea.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'pickle_idea.py'), ('C:\\Python27\\lib', 'datetime'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'pickle_idea.py'), ('C:\\Python27\\lib', 'pickle.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'pickle_idea2.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'pickle_idea2.py'), ('C:\\Python27\\lib', 'datetime'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'pickle_idea2.py'), ('C:\\Python27\\lib', 'pickle.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'wordfreqCMD.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'wordfreqCMD.py'), ('C:\\Python27\\lib', 'collections.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'wordfreqCMD.py'), ('C:\\Python27\\lib', 'operator'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'wordfreqCMD.py'), ('C:\\Python27\\lib', 'os.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'wordfreqCMD.py'), ('C:\\Python27\\lib', 'string.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'wordfreqCMD.py'), ('C:\\Python27\\lib', 'sys'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'wordfreqCMD.py'), ('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app', 'pickle_idea.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_add_word.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_add_word.py'), ('C:\\Python27\\lib', 'random.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_add_word.py'), ('C:\\Python27\\lib', 'string.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_add_word.py'), ('C:\\Python27\\lib', 'time'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_add_word_and_essay_does_not_change.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_add_word_and_essay_does_not_change.py'), ('C:\\Python27\\lib', 'random.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_add_word_and_essay_does_not_change.py'), ('C:\\Python27\\lib', 'string.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_add_word_and_essay_does_not_change.py'), ('C:\\Python27\\lib', 'time'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_delete_word.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_delete_word.py'), ('C:\\Python27\\lib', 'random.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_delete_word.py'), ('C:\\Python27\\lib', 'string.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_delete_word.py'), ('C:\\Python27\\lib', 'time'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_login.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_login.py'), ('C:\\Python27\\lib', 'random.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_login.py'), ('C:\\Python27\\lib', 'string.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_login_security_fix.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_login_security_fix.py'), ('C:\\Python27\\lib', 'random.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_login_security_fix.py'), ('C:\\Python27\\lib', 'string.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_next_essay.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_next_essay.py'), ('C:\\Python27\\lib', 'random.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_next_essay.py'), ('C:\\Python27\\lib', 'string.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_next_essay.py'), ('C:\\Python27\\lib', 'time'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_page_position.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_page_position.py'), ('C:\\Python27\\lib', 'random.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_signup.py'), (None, None))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_signup.py'), ('C:\\Python27\\lib', 'random.py'))
  (('E:\\Desktop\\\xd1\xa7\xd0\xa3\\\xc8\xfd\xc9\xcf\\\xc8\xed\xbc\xfe\xcc\xe5\xcf\xb5\xbd\xe1\xb9\xb9\\englishpal\\app\\test', 'test_signup.py'), ('C:\\Python27\\lib', 'string.py'))
  
  ```

  

- 1.dot

  ```
  # This file was generated by sfood-graph.
  
  strict digraph "dependencies" {
      graph [
          rankdir = "LR",
          overlap = "scale",
          size = "8,10",
          ratio = "fill",
          fontsize = "16",
          fontname = "Helvetica",
          clusterrank = "local"
          ]
  
         node [
             fontsize=7
             shape=ellipse
  //           style=filled
  //           shape=box
         ];
  
  //     node [
  //         fontsize=7
  //       style=ellipse
  //     ];
  
  "UseSqlite.py"  [style=filled];
  "UseSqlite.py" -> "sqlite3";
  "WordFreq.py"  [style=filled];
  "WordFreq.py" -> "string.py";
  "WordFreq.py" -> "wordfreqCMD.py";
  "difficulty.py"  [style=filled];
  "difficulty.py" -> "math";
  "difficulty.py" -> "pickle.py";
  "difficulty.py" -> "wordfreqCMD.py";
  "main.py"  [style=filled];
  "pickle_idea.py"  [style=filled];
  "pickle_idea.py" -> "datetime";
  "pickle_idea.py" -> "pickle.py";
  "pickle_idea2.py"  [style=filled];
  "pickle_idea2.py" -> "datetime";
  "pickle_idea2.py" -> "pickle.py";
  "wordfreqCMD.py"  [style=filled];
  "wordfreqCMD.py" -> "collections.py";
  "wordfreqCMD.py" -> "operator";
  "wordfreqCMD.py" -> "os.py";
  "wordfreqCMD.py" -> "string.py";
  "wordfreqCMD.py" -> "sys";
  "wordfreqCMD.py" -> "pickle_idea.py";
  "test_add_word.py"  [style=filled];
  "test_add_word.py" -> "random.py";
  "test_add_word.py" -> "string.py";
  "test_add_word.py" -> "time";
  "test_add_word_and_essay_does_not_change.py"  [style=filled];
  "test_add_word_and_essay_does_not_change.py" -> "random.py";
  "test_add_word_and_essay_does_not_change.py" -> "string.py";
  "test_add_word_and_essay_does_not_change.py" -> "time";
  "test_delete_word.py"  [style=filled];
  "test_delete_word.py" -> "random.py";
  "test_delete_word.py" -> "string.py";
  "test_delete_word.py" -> "time";
  "test_login.py"  [style=filled];
  "test_login.py" -> "random.py";
  "test_login.py" -> "string.py";
  "test_login_security_fix.py"  [style=filled];
  "test_login_security_fix.py" -> "random.py";
  "test_login_security_fix.py" -> "string.py";
  "test_next_essay.py"  [style=filled];
  "test_next_essay.py" -> "random.py";
  "test_next_essay.py" -> "string.py";
  "test_next_essay.py" -> "time";
  "test_page_position.py"  [style=filled];
  "test_page_position.py" -> "random.py";
  "test_signup.py"  [style=filled];
  "test_signup.py" -> "random.py";
  "test_signup.py" -> "string.py";
  
  
  }
  ```

  

- 依赖关系

  ![sna](E:\Desktop\学校\三上\软件体系结构\dot\sna.png)



### 任务分析小结

我们组没有对项目进行很好的重构，项目可能没有特别规范，亦或者**python2 的snakefood 无法很好的 解析 python3 的项目**，导致生成的依赖关系**有些偏差**。不过通过上图依然可以较好的对项目进行 Module-level dependency analysis。





## 任务二 class-level or function-level dependency analysis（By  Mermaid）


### pycallgraph 分析 （on Windows）

- 安装 pycallgraph

  ``pip3 install pycallgraph``

- 安装 graphviz ~~windows上 貌似 直接pip下载无法调用~~

[graphviz.msi 下载地址](https://graphviz.gitlab.io/_pages/Download/windows/graphviz-2.38.msi)

- 对单一文件生成图像

  ``python3 "C:\******\Python\Python37\Scripts\pycallgraph" graphviz "C:\********\app\****.py"``

  但还是由于没有重构完全的原因，导致**只有部分文件可以得到依赖图片**

  并且 不同py文件间的方法引用也无法识别

  

  **pickle_idea.py**

  ![pickle_idea](E:\Desktop\学校\三上\软件体系结构\dot\uml\pickle_idea.png)

  

  **UseSqlite.py**



![UseSqlite](E:\Desktop\学校\三上\软件体系结构\dot\uml\UseSqlite.png)



~~不想分析了，人麻了~~



### Pyreverse 分析（on Ubuntu）

- 安装 pylint (Pyreverse 为内置函数)

  ``pip install pylint``

- 安装 graphviz (绘图工具)

  ``pip install graphviz``

- 生成依赖 ~~指令已经忘了，虚拟机上忘记截图，结果不好，已经麻了~~

**packages.dot**

```
digraph "packages" {
charset="utf-8"
rankdir=BT
"0" [label="/home/qzs/1/englishpal/app/UseSqlite.py", shape="box"];
"1" [label="/home/qzs/1/englishpal/app/WordFreq.py", shape="box"];
"2" [label="/home/qzs/1/englishpal/app/__init__.py", shape="box"];
"3" [label="/home/qzs/1/englishpal/app/difficulty.py", shape="box"];
"4" [label="/home/qzs/1/englishpal/app/pickle_idea.py", shape="box"];
"5" [label="/home/qzs/1/englishpal/app/pickle_idea2.py", shape="box"];
"6" [label="/home/qzs/1/englishpal/app/wordfreqCMD.py", shape="box"];
}
```

**packages.png**

![packages](E:\Desktop\学校\三上\软件体系结构\dot\packages.png)



**classes.dot**

```
digraph "classes" {
charset="utf-8"
rankdir=BT
"0" [label="{InsertQuery|query\l|instructions()\l}", shape="record"];
"1" [label="{RecordQuery|query\l|format_results()\lget_results()\linstructions()\l}", shape="record"];
"2" [label="{Sqlite3Template|conn\ldb_fname\lparameters\lquery\lresults\l|connect()\ldo()\ldo_with_parameters()\lformat_results()\linstructions()\linstructions_with_parameters()\loperate()\loperate_with_parameters()\l}", shape="record"];
"3" [label="{WordFreq|s\l|get_freq()\l}", shape="record"];
"0" -> "2" [arrowhead="empty", arrowtail="none"];
"1" -> "2" [arrowhead="empty", arrowtail="none"];
}
```



**classes.png**

![classes](E:\Desktop\学校\三上\软件体系结构\dot\classes.png)

### 手绘 class-level

- 依赖

```
classDiagram
    pickle_idea ..> pickle
    pickle_idea ..> datetime
    pickle_idea2 ..> pickle
    pickle_idea2 ..> datetime
    Sqlite3Template ..> sqlite3
    Sqlite3Template <|-- InsertQuery
    Sqlite3Template <|-- RecordQuery
    wordfreqCMD ..> pickle_idea
    wordfreqCMD ..> collections
    wordfreqCMD ..> string
    wordfreqCMD ..> os
    wordfreqCMD ..> sys
    WordFreq ..> wordfreqCMD
    WordFreq ..> string
    difficulty..> wordfreqCMD
    difficulty..> math
    difficulty..> pickle
    main ..> wordfreqCMD
    main ..> WordFreq
    main ..> InsertQuery
    main ..> RecordQuery
    main ..> pickle_idea
    main ..> pickle_idea2
    main ..> os
    main ..> random
    main ..> glob
    main ..> datetime
    main ..> Flask
    main ..> difficulty

    class difficulty{
    +load_record(pickle_fname)
    +difficulty_level_from_frequency(word, d)
    +get_difficulty_level(d1, d2)
    +revert_dict(d)
    +user_difficulty_level(d_user, d)
    +text_difficulty_level(s, d)
}
    class pickle_idea{
    +lst2dict(lst, d)
    +dict2lst(d)
    +merge_frequency(lst1, lst2)
    +load_record(pickle_fname)
    +save_frequency_to_pickle(d, pickle_fname)
    +unfamiliar(path,word)
    +familiar(path,word)
}
    class pickle_idea2{
    +lst2dict(lst, d)
    +deleteRecord(path,word)
    +dict2lst(d)
    +merge_frequency(lst1, lst2)
    +load_record(pickle_fname)
    +save_frequency_to_pickle(d, pickle_fname)
}

    class InsertQuery{
    +instructions(self, query)
}
    class RecordQuery{
    +instructions(self, query)
    +format_results(self)
    +get_results(self)
}
    class WordFreq{
    +__init__(self, s)
    +get_freq(self)
}
    class wordfreqCMD{
    +freq(fruit)
    +youdao_link(s)
    +file2str(fname)
    +remove_punctuation(s)
    +sort_in_descending_order(lst)
    +sort_in_ascending_order(lst)
    +make_html_page(lst, fname)
}
    class main{
    +get_random_image(path)
    +get_random_ads()
    +total_number_of_essays()
    +load_freq_history(path)
    +verify_user(username, password)
    +add_user(username, password)
    +check_username_availability(username)
    +get_expiry_date(username)
    +within_range(x, y, r)
    +get_article_title(s)
    +get_article_body(s)
    +get_today_article(user_word_list, articleID)
    +appears_in_test(word, d)
    +get_time()
    +get_question_part(s)
    +get_answer_part(s)
    +get_flashed_messages_if_any()
    +highlight(text, word)
    +user_reset(username)
    +mark_word()
    +mainpage()
    +user_mark_word(username)
    +unfamiliar(username,word)
    +familiar(username,word)
    +deleteword(username,word)
    +userpage(username)
    +signup()
    +login()
    +logout()
}    
    class Sqlite3Template{
    +__init__(self, db_fname)
    +connect(self, db_fname)
    +instructions(self, query_statement)
    +operate(self)
    +format_results(self)
    +do(self)
    +instructions_with_parameters(self, query_statement, parameters)
    +do_with_parameters(self)
    +operate_with_parameters(self)
}

```



- 依赖图

  ![hand](E:\Desktop\学校\三上\软件体系结构\dot\uml\hand.png)

## Analizy



