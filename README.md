# PackApk: Python打包apk脚本

`auto.py`和`auto.config`是使用Python写的脚本，主要用来从Git拉项目代码后打包成apk

## Usage

1.环境准备：配置好python(2.x或3.x)、gradle环境

2.将`auto.py` 和 `auto.config` 文件放在同一级目录下。

3.然后配置`auto.config`文件：

- `Root_SDK_Dir` 是你的SDK的绝对路径
- `git_clone_address` 是你的Git地址
- `git_branch_name` 要拉取的远端分支名
- `assembleRelease` boolean值，是否打release包
- `base_file_dir` 是一个绝对路径，可随便填
- `create_dir_name` 将在`base_file_dir`生成一个目录，用于存放项目代码和打出来的APK文件
- `create_code_dir_name` 项目代码存放的目录名
- `create_apk_dir_name` APK文件存放目录名
- `apk_name` 自定义apk的名字，必须带后缀`.apk`

配置好后你就可以使用python命令行运行该脚本，等待打包完成。

4.打开控制台，进入当前项目的目录，然后执行：

```python
   python auto.py
```
或者
```python
   python3 auto.py
```
