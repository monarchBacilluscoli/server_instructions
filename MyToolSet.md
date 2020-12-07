# My Toolset

这一部分是进行该工程使用过的工具总述。

## The Project
### 工程外与工程相关的工具
#### VSCode
通用的编辑器，各种扩展插件实现了对各类语言的各种编译调试等的工具（c++的G++、GDB，Latex的latexmk、Conda）的流畅调用，实现了F5调试代码的舒适体验并且支持基于SSH的远程调试。是本人在Linux、Windows、Mac诸平台编写C++、Latex、Python、HTML、JS等代码的通用编辑器，甚至可以画些示意图啥的。
#### CMake
跨平台做代码工程管理的玩意，采用统一且友好的语法包办了这个工程的编译。
#### Make
了解一点即可，CMake想必是在这玩意的基础上进行的抽象。其实就是处理编译依赖的自动化工具。
#### G++
c++的编译器，具体和GCC的关系啥的可以自己查，g++这个名字最不容易误解。
#### GDB
Linux平台的调试器，交互式的CLI程序，简单易用，似乎并不只适用于C++，但是这个工程只是c++。

### 工程内的工具
主要指这个工程依赖的几个库。sc2clientAPI主要依赖于几个东西：
#### Protocol Buffer
google写的用于序列化和反序列化数据的库，类比json、XML等，可以用protobuffer自己的语法在.proto中定义各个字段然后生成各类语言（C++、python等等）的代码并基于这些代码，使用它的工程可以与之高效交互，不用拿着json等文件边对照边写unit.getfield("health")，而是直接unit.GetHealth()。当然最重要的，这种方法和其他方法比号称会十分地快。
#### SDL2
Simple DirectMedia Layer 2, 多媒体库，提供对于图形音频控制等的API，非必须，用于SC2 C++API中的feature layer的显示。
#### Civetweb 
这玩意可以用来快速搭建网站服务器，应该包装了一些实用的处理TCP/IP连接的玩意。具体...我跳过了，看了一点更底层的Linux网络部分，以及TCP/IP的内容。

### 其他值得一提的工具
#### Python
“Life is short, use Python”
##### Conda
Anaconda的图形界面看着就费劲，我就处理一下包依赖，天天打交道的就是conda install xxxx, conda update，我要图形干啥？还那么大。我用Miniconda。
##### Keras
Python下非常方便易用的机器学习库，包装了Tenserflow、Pythorch等后端，前端就是很简单的语法，半天即可掌握工具，开箱即用，简直神器。
#### Git
我好久不用Github Desktop或者别的什么独立的Git图形工具了。

### 文章的工具
#### Latex
学就对了，入门书籍 + texdoc命令，或者上网查。
#### Python
“Life is short, use Python”, again.
##### Seaborn
非常方便易用的绘图库，在matplotlib之上又进行了一次封装，十分易于上手，上手时只要注意区分几个简单的概念：figure level/axes level，以及Pandas的long-form/wide-form数据类型即可。
##### Pandas.dataFrame
表格一样直观，还附带各种方便的数据处理工具及语法。唯一注意数据类型变成object的问题。

### vscode插件选编
常驻的：
#### Git Graph
vscode内即可图形查看git log. 不过我推荐先试一下git log也未尝不可。
#### Remote-SSH
远程开发必备。
#### Better Comments
好看你的注释。

### Linux系统里的好东西
看前面的说明吧
