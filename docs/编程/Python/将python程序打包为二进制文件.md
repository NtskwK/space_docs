# nuitka

示例中的参数包含显示以下功能：

`显示进度`：显示编译进度

`独立运行环境`：以便程序在没有python的机器上运行

`单个exe文件`：将所有文件打包到一个exe文件中（在涉及win api操作时应谨慎使用，因为该行为可能导致杀毒软件误杀）

`启用插件`：允许使用upx压缩exe文件

`假设下载依赖项时选择yes`：允许在依赖不完全的机器上下载依赖项

`不跟随导入`：允许不跟随导入的模块

`启用LTO`：允许启用LTO优化

`mingw64`：允许使用mingw64编译器进行编译

```bash
nuitka --show-progress --standalone --onefile --enable-plugin=upx --assume-yes-for-downloads --nofollow-imports --lto=yes --mingw64 main.py
```