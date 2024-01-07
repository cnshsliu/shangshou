# Shangshou 上手 大道至简

为Jerome

进入AI的世界

## 目的

从零开始，成为一名AI工程师，未来在AI领域有独创能力。

## 起步要求

尽量做到极低

在计算机知识上，只要会打字，会基本的计算机操作即可

要求有基本的英语阅读能力，在ChatGPT的协助下，可以高效阅读英文文档

## 方法

熟悉在学校里学习不到的各种实际工作中用到的工具。

大道至简、简明扼要，每个知识点说明：

1. 是什么
2. 有什么
3. 怎么操作

## 开源

1. 开源， 指的是软件的源代码，是公开的，任何人都可以查看、修改、使用、分发。
2. 开源软件作者，一般会在软件的源代码中，附上一份开源协议，告诉使用者，这个软件，可以做什么，不能做什么。
3. 比如，GPL3.0协议，就是一种开源协议，它规定，使用者，可以免费使用、修改、分发，但是，如果使用者，将这个软件，作为自己的产品，分发给其他人，那么，使用者，必须将自己的产品，也开源出来。
4. 再比如， MIT协议，也是一种开源协议，它规定，使用者，可以免费使用、修改、分发，但是，使用者，不需要开源自己的产品。
5. 开源软件作者，可以采用多种开源协议，也可以采用多种开源协议的组合，比如，Linux内核，就采用了多种开源协议的组合。 也可以定义自己的开源协议（但写好文字定义其实很困难，字斟句酌，所以，一般选择一个现有的开源协议）

## 操作系统

1. 故名思义，操作系统，就是用来操作计算机的一套系统软件。
2. 常用的操作系统有Windows、MacOS、Linux
3. Windows多用于办公场景，MacOS多用于创作场景，Linux多用于服务器场景
4. Linux且有天然的开源属性和开放属性，有丰富的开发工具链，因此，在AI开发、运行领域，Linux是主流操作系统
5. Linux的发行版有很多，常用的有Ubuntu、CentOS、Debian、RedHat。
6. 所谓发行版，是说Linux内核是一套，但是，不同的厂商，会在内核上，加入自己的一些东西，形成不同的发行版。
7. 发行版的选择，主要看个人喜好，但是，建议选择Ubuntu，因为，Ubuntu是最流行的发行版，有最多的用户，有最多的资料，有最多的工具，有最多的支持。
8. 发行版之间存在依赖，任何人都可以使用一个发行版，来制作自己的发行版，这就是所谓的衍生版，比如，Ubuntu衍生出了Kubuntu、Xubuntu、Lubuntu、Ubuntu Kylin等等。而Ubuntu自身的上游是Debian，Debian的版本更新频度慢，系统非常稳定。
9. Mac OSX是基于BSD的，BSD是Unix的衍生版，BSD的上游是Unix，Unix是最早的操作系统，是所有操作系统的鼻祖，Unix的发行版有很多，比如，Solaris、AIX、HP-UX等等，但是，Unix的发行版，都是收费的，因此，BSD是Unix的开源版本，Mac OSX是基于BSD的，因此，Mac OSX也是收费的。
10. Mac OSX和Linux一样，都是基于Unix的，因此，Mac OSX和Linux具有类似的工具链，加上它的图形界面非常方便，因此，往往称为需要兼顾方便性和Unix工具链依赖性的程序员的首选
11. Windows系统也慢慢明白支持Linux工具链的重要性，因此，Windows 10开始，支持了Linux子系统，可以在Windows上运行Linux工具链，但毕竟基因不同，Windows往往是程序员的备选

## 虚拟机

1. 虚拟机，是一种软件，可以在一台物理计算机上（称为宿主机），虚拟出多台计算机，每台计算机，都有自己的操作系统，自己的磁盘，自己的网络，自己的软件。 虚拟机之上，一般不再继续第二层虚拟化
2. 虚拟机带来灵活性，可以在一台宿主机上，使用不同的操作系统，用于体验、开发或正式运行。比如，可以在Windows上，运行Linux，也可以在MacOS上，运行Linux。
3. 公有云上提供的“云服务器”，就是云服务商在自己的物理机（宿主机）上，虚拟出来的虚拟机，分配给用户使用。

## 容器

1. 容器跟虚拟机类似，都是一种软件，可以在一台物理计算机上（称为宿主机），虚拟出多个计算机，每个计算机，都有自己的操作系统，自己的磁盘，自己的网络，自己的软件。
2. 容器跟虚拟机不同，容器不是虚拟出来的计算机，而是虚拟出来的进程
3. 容器给到用户一个幻觉，就是用户在使用一个独立的计算机，但是，实际上，容器是宿主机上的一个进程，跟宿主机上的其他进程，共享操作系统内核，共享宿主机的资源，比如，CPU、内存、磁盘、网络等等。
4. 容器比虚拟机更轻量，更灵活，更快速，更易于管理，因此，容器是云原生时代的主流。
5. 容器技术常用的是Docker，Docker是一种容器技术，Docker的容器，可以在Windows、MacOS、Linux上运行，也可以在公有云上运行，也可以在私有云上运行。其它容器技术包括Containerd等。
6. 容器里面的软件，可以打包成镜像，镜像可以分发给其他人，也可以上传到公有云，也可以上传到私有云，也可以上传到Docker Hub，供其他人下载使用。
7. 镜像的制作，可以通过Dockerfile来定义，Dockerfile是一种文本文件，里面定义了如何制作镜像，比如，从哪个镜像开始，安装哪些软件，运行哪些命令等等。
8. 镜像实例化后，就是容器，容器可以运行，也可以停止，也可以删除，也可以重启，也可以暂停，也可以恢复。

### Docker Cheat Sheet

1. https://docs.docker.com/get-started/docker_cheatsheet.pdf
2. https://dockerlux.github.io/pdf/cheat-sheet-v2.pdf
3. https://phoenixnap.com/kb/docker-commands-cheat-sheet
4. https://devopscycle.com/blog/the-ultimate-docker-cheat-sheet/

## Shell

1. Unix系统的命令行，称为Shell. 用户通过命令行，跟操作系统交互，执行命令。
2. Shell是一种脚本语言，可以用来编写脚本，用来执行一系列命令。
3. Linux系统的Shell，有很多种，比如，Bash、Zsh、Fish等等，不同的Shell，有不同的特性，但是，基本的命令，都是一样的。Bash是各个Linux发行版的标配，Zsh在MacOSX上已成为标配。 Zsh用起来更方便，且兼容Bash脚本的语法

### Bash Cheat Sheet

如何通过Bash来操作Linux系统
[Shell Cheat Sheet](https://github.com/RehanSaeed/Bash-Cheat-Sheet)
[Linux Bash Shell Cheat Sheet](https://hpc.ua.edu/wp-content/uploads/2022/02/Linux_bash_cheat_sheet.pdf)

### Bash Scripting Cheat Sheet

如何写Linux Bash脚本， 来执行一系列命令
[Bash scripting cheatsheet](https://devhints.io/bash)

### Bash/Zsh启动脚本

1. Linux是多用户操作系统，每个用户都有自己的家目录，每个用户都可以有自己的启动脚本，用来在用户登录时，自动执行一些命令，比如，设置环境变量，设置别名等等。
2. Bash的启动脚本是~/.bashrc，Zsh的启动脚本是~/.zshrc，这两个文件，都是隐藏文件，可以通过ls -a命令来查看。 (Linux上，文件和目录以点开头的，ls列不出来，要用ls -a来列出来）

### Linux软件包

1. Ubuntu系统的软件，一般都是通过apt-get命令来安装，apt-get命令，会从Ubuntu的软件源里，下载软件包，然后安装。
2. 这一点与Windows的软件安装方式不同，Windows的软件，一般都是从软件官网下载安装包，然后安装。

### Homebrew

1. Homebrew的命令是brew，Homebrew是MacOSX的包管理器，可以用来安装软件，类似于Linux的apt-get命令。
2. 在MacOSX上，可以通过Homebrew来安装Linux的软件，比如，通过brew install git，来安装git命令行工具。

## 编程语言

1. 编程语言有解释型和编译型两类，编译型语言，需要先编译成机器码，再执行，比如，C、C++、Go、Rust等等。解释型语言，不需要编译，直接执行，比如，Python、Ruby、JavaScript、PHP等等。
2. 编译后的机器码运行效率一般比解释型要高, 但计算机性能越来越高，解释型语言的性能已经足够，而且，解释型语言的开发效率更高，因此，解释型语言已经成为主流。
3. Python由于语法简单，易于学习，且有丰富的第三方库，因此，成为AI领域的主流编程语言。
4. Javascript由于浏览器的普及，成为前端开发的主流编程语言。
5. Node.JS是Javascript的运行时，可以在服务器上运行Javascript，因此，Node.JS成为服务器端开发的主流编程语言。
6. TypeScript是Javascript的超集，可以编译成Javascript，因此，TypeScript成为前后端全栈开发的主流编程语言。

## 常用的跟语言相关的工具：

1. 编辑器： 用于便携代码
2. 编译器： 用于编译代码
3. 调试器： 用于调试代码
4. Lint: 用于检查代码
5. Prettier： 用于格式化代码

VSCode这种集成开发环境中，以上工具都自带或者通过安装插件来使用。
NeoVIM中通过安装插件来使用。

## 编辑器

1. 编辑器，是用来编辑文本的软件，比如，记事本、Word、Pages等等。
2. 程序员用的编辑器，一般是专门用来编辑代码的，比如，Sublime Text、Atom、VSCode、Vim、Emacs等等。
3. NeoVIM是Vim的升级版，Vim是Vi的升级版，Vi是Unix系统自带的编辑器，Vim和NeoVIM都是命令行编辑器，可以在终端里使用，也可以在GUI里使用。
4. 在系统里，往往由于没有图形界面，因此，需要掌握vim的基础操作
5. 推荐掌握VSCode和NeoVIM， VSCode方便，NeoVIM高效，两者可以互补。

## VIM Cheet Sheet

1. [Vim cheatsheet](https://devhints.io/vim)

2. [Another Vim Cheat Sheet](https://vim.rtorr.com/)

## NeoVIM

Neovim是VIM的重写版，兼容Vim，但是，更加高效，更加易于扩展，更加易于配置，更加易于使用。

早器的Uninx系统都带vi，现在的Linux都带Vim，在shell中运行

```
vim
```

即可

Neovim则需要安装， 可以在shell中运行

```
brew install neovim
···

[Home - NeovimNeovim](https://neovim.io/)

很多人需要VSCode的图形界面，但是，在编辑文件时，又想用Vim的高效，可以使用VSCode的NeoVim插件

[GitHub - vscode-neovim/vscode-neovim: Vim mode for VSCode, powered by Neovim](https://github.com/vscode-neovim/vscode-neovim)

## Git 和 Github

1. Git是一种版本控制系统，可以用来管理代码，可以用来管理文档，可以用来管理任何文本文件。
2. Git的作者是Linus Torvalds，是Linux的作者，因此，Git是Linux的标配，也是AI工程师的标配。
3. Git的命令行工具，是git，可以在命令行里使用，也可以在GUI里使用。
4. Git是分布式的，每个人都可以有自己的Git仓库，也可以有自己的分支，也可以有自己的提交，也可以有自己的历史。
5. Github是一个网站，是一个代码托管网站

   [Git Cheet Sheet](https://education.github.com/git-cheat-sheet-education.pdf)

   [Atlassian Git Cheet Sheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)

   [Gitlab's Git Cheet Sheet](https://about.gitlab.com/images/press/git-cheat-sheet.pdf)

## Python 环境

1. Python安装后，会在系统里安装一个Python解释器，可以在命令行里执行Python代码。
2. Python有很多版本，在系统里在多个版本间切换，非常麻烦，因此，要使用pyenv来建立Python的虚拟环境，每个虚拟环境，都有自己的Python版本，自己的Python库，自己的Python脚本。
3. Python的大版本有2和3，Python2已经不再维护，因此，要使用Python3， 但在工作中，可能会遇到一些库必须依赖Python2。

### Pyenv Github

[GitHub - pyenv/pyenv: Simple Python version management](https://github.com/pyenv/pyenv)

[pyenv/pyenv 安装](https://github.com/pyenv/pyenv?tab=readme-ov-file#installation)

### pip

pip是Python的包管理器，可以用来安装Python的库，类似于Linux的apt-get命令。

在开源软件的世界里，不同的平台环境都有自己的包管理器，比如，Linux的apt-get，MacOSX的Homebrew，Python的pip，Node.JS的npm，Ruby的gem，Java的maven，Go的go get等等。

[A Pip Cheat Sheet](https://ugoproto.github.io/ugo_py_doc/pdf/Pip-Cheatsheet.pdf)
```
