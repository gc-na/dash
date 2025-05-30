# [中文] Debian Almquist Shell (dash) ls 用法等价: 列出目录内容

## 概述
`ls` 命令用于列出指定目录中的文件和子目录。它是 Unix 和类 Unix 系统中最常用的命令之一，帮助用户快速查看文件系统的内容。

## 用法
基本语法如下：
```
ls [选项] [参数]
```

## 常用选项
- `-l`：以长格式显示文件信息，包括权限、所有者、文件大小和修改时间。
- `-a`：显示所有文件，包括以点（.）开头的隐藏文件。
- `-h`：与 `-l` 一起使用时，以人类可读的格式显示文件大小（例如 KB、MB）。
- `-R`：递归列出所有子目录的内容。
- `-t`：根据修改时间排序文件，最新的文件排在前面。

## 常见示例
1. 列出当前目录的文件：
   ```bash
   ls
   ```

2. 列出当前目录的所有文件，包括隐藏文件：
   ```bash
   ls -a
   ```

3. 以长格式显示当前目录的文件信息：
   ```bash
   ls -l
   ```

4. 以人类可读的格式显示文件大小：
   ```bash
   ls -lh
   ```

5. 递归列出所有子目录的内容：
   ```bash
   ls -R
   ```

6. 根据修改时间排序文件：
   ```bash
   ls -lt
   ```

## 小贴士
- 使用 `ls -lh` 可以更方便地查看文件大小，特别是在处理大文件时。
- 结合使用多个选项，例如 `ls -la`，可以同时查看所有文件及其详细信息。
- 如果需要查看特定目录的内容，可以在命令后指定目录路径，例如 `ls /path/to/directory`。