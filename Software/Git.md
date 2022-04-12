# Git

git安装时会自带一个git bash工具，用起来感觉比cmd方便。可今天发现一个问题，用git bash无法创建文件夹和文件。在cmd下，只需要 md+文件夹名 就可以创建一个文件夹，可md在git bash下是无效的命令。

原因是cmd和git bash是两个完全不同的工具，cmd用的是Windows自己的命令，而git bash用的是linux下的命令。

在git bash新建文件夹命令是 mkdir+文件夹名。

## 新建文件有两种方式：

1，touch+文件名，直接新建一个文件

2，vi+文件名，新建一个文件并进入编辑状态（如果文件已存在，则直接进入编辑状态）

vi其实是linux的一个文本编辑器，所以 vi+文件名 后，其实是进入vi程序了。vi有两种模式，编辑模式和命令模式

### 1、vi & vim 有两种工作模式：

（1） 命令模式：接受、执行 vi & vim 操作命令的模式，打开文件后的默认模式；

（2） 编辑模式：对打开的文件内容进行 增、删、改 操作的模式；

#在编辑模式下按下 ESC 键，回退到命令模式。

### 2、创建、打开文件：$ vi 文件名

（1）使用 vi 加 文件路径（或文件名）的模式打开文件，如果文件存在则打开现有文件，如果文件不存在则新建文件，并在终端最下面一行显示打开的是一个新文件。

（2）键盘输入字母 “i”或“Insert”键进入最常用的插入编辑模式。

### 3、保存文件：

（1）在插入编辑模式下编辑文件。

（2）按下 “ESC” 键，退出编辑模式，切换到命令模式。

（3）在命令模式下键入"ZZ"或者":wq"保存修改并且退出 vi 。

（4）如果只想保存文件，则键入":w"，回车后底行会提示写入操作结果，并保持停留在命令模式。

### 4、放弃所有文件修改：

（1）放弃所有文件修改：按下 "ESC" 键进入命令模式，键入 ":q!" 回车后放弃修改并退出vi。

（2）放弃所有文件修改，但不退出 vi ，即回退到文件打开后最后一次保存操作的状态，继续进行文件操作：按下 "ESC" 键进入命令模式，键入 ":e!" ，回车后回到命令模式。

## Command line instructions

### You can also upload existing files from your computer using the instructions below.

`Git global setup`
```
git config --global user.name
git config --global user.email 
```

### Create a new repository

```
git clone https://xxx.git
cd surgio
git switch -c main
touch [README.md](http://readme.md/)
git add [README.md](http://readme.md/)
git commit -m "add README"
git push -u origin main
```

### Push an existing folder

```
cd existing_folder
git init --initial-branch=main
git remote add origin https://xxx.git
git add .
git commit -m "Initial commit"
git push -u origin main
```

### Push an existing Git repository
```
cd existing_repo
git remote rename origin old-origin
git remote add origin https://xxx.git
git push -u origin --all
git push -u origin --tags
```
