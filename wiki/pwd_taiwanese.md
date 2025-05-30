# [台灣] Debian Almquist Shell (dash) pwd 使用法: 顯示當前工作目錄

## Overview
`pwd` 命令用於顯示當前工作目錄的完整路徑。這在使用命令行時非常有用，因為它可以幫助你確認你目前所在的目錄位置。

## Usage
基本語法如下：
```
pwd [options]
```

## Common Options
- `-L`：顯示邏輯路徑，這是預設選項。
- `-P`：顯示物理路徑，這會顯示實際的路徑，不會遵循符號鏈接。

## Common Examples
1. 顯示當前工作目錄：
   ```bash
   pwd
   ```

2. 顯示物理路徑：
   ```bash
   pwd -P
   ```

3. 顯示邏輯路徑（預設行為）：
   ```bash
   pwd -L
   ```

## Tips
- 使用 `pwd` 前，確保你已經在命令行中進入了某個目錄，這樣才能正確顯示路徑。
- 結合其他命令使用，例如在腳本中，可以用 `pwd` 獲取當前目錄並將其存儲到變數中。