# VS Code

一、**为Windows安装C编译器MinGW-W64 GCC**, 链接：[https://winlibs.com/](https://winlibs.com/)

二、**配置环境变量**

1. 下载后是一个压缩文件，将它解压到指定的文件夹，可以是C盘
2. 点开，进入它的“bin”子文件夹，然后复制路径“C:\mingw64\bin”
3. 然后右键点击“此电脑”，选择最下面的子菜单“属性”
4. 调出“系统”对话框，然后点击左方的“高级系统设置”按钮，调出“系统属性对话框”
5. 在“系统属性”对话框中的“高级”选项卡下点击“环境变量”按钮，调出“环境变量”对话框
6. 在“环境变量”对话框中，选中“Path”，点击“编辑”按钮，调出“编辑环境变量”对话框
7. 在“编辑环境变量”对话框中点击“新建”按钮，在下方粘贴上面复制的mingw64的地址
8. 依次点击“确定”按钮，完成C编译器的安装和环境变量配置。如果配置成功，同时按下键盘上的“win+r“键，在出现的”运行“对话框中输入”cmd“回车
9. 在随后出现的”cmd.exe"窗口中，输入“gcc -v"命令，会出现gcc的版本号，说明安装配置成功

三、**安装并配置Visual Studio Code**

1. 下载VSCode，下载地址为：[https://code.visualstudio.com/](https://link.zhihu.com/?target=https%3A//code.visualstudio.com/)，在网页中点击”Download for Windows“按钮即可下载。当然，还可以点击按钮右侧紧挨的向下的箭头选择不同操作系统的VSCode版本
2. 下载下来是一个exe的安装文件，”VSCodeUserSetup-x64-1.53.2.exe“。如果你觉得下载速度慢，可以复制下载链接然后使用迅雷等下载工具下载 
3. VSCode的安装比较简单，根据提示一路傻瓜式安装，完成后在开始菜单下就会有“Visual Studio Code”了，点击打开
4. 打开后，如下图。左侧边栏是几个快速的按钮，点击最下面的“Extensions”（扩展）按钮
5. 在随后出现的”扩展市场“的搜索框中输入”C/C++“，在随后出现的列表中选择对应的扩展，确认是Microsoft家的，就点击”Install“按钮即可安装
6. 安装完”C/C++"扩展后，安装“Code Runner”扩展，方法相同
7. 俩扩展安装完成后，是对“Code Runner”扩展的配置，在“File”菜单下找到“Preference”再找到“Settings”子菜单
8. 在随后的Settings页面中，将“Run Code Configuration”中的“Run In Terminal"、"Save File Before Run"前面的复选框选中
9. VSCode及其扩展的安装、位置完成

四、**史上最全vscode配置使用教程**

链接：[https://zhuanlan.zhihu.com/p/113222681](https://zhuanlan.zhihu.com/p/113222681)

五、**备份好的pdf文件**：`（百度网盘）VS Code Basic Config.pdf`

`VS Code：4个中文乱码问题及解决方法`

链接：[https://www.jianshu.com/p/6a2c21cc07bb](https://www.jianshu.com/p/6a2c21cc07bb)
