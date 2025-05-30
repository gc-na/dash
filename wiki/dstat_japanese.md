# [日本語] Debian Almquist Shell (dash) dstat の使い方: システムリソースの監視

## Overview
dstat コマンドは、システムのリソース使用状況をリアルタイムで監視するためのツールです。CPU、メモリ、ディスク、ネットワークなどのパフォーマンスを簡単に確認することができます。

## Usage
基本的な構文は以下の通りです。

```bash
dstat [options] [arguments]
```

## Common Options
- `-c` : CPU 使用率を表示します。
- `-d` : ディスクの読み書き速度を表示します。
- `-n` : ネットワークの送受信速度を表示します。
- `-m` : メモリの使用状況を表示します。
- `-t` : 時間を表示します。

## Common Examples
以下に、dstat コマンドの実用的な例をいくつか示します。

### CPU 使用率の表示
```bash
dstat -c
```

### ディスクの読み書き速度の表示
```bash
dstat -d
```

### ネットワークの送受信速度の表示
```bash
dstat -n
```

### CPU、メモリ、ディスク、ネットワークの同時表示
```bash
dstat -cdmn
```

### 時間を含めた全リソースの表示
```bash
dstat -cmdn -t
```

## Tips
- dstat を使用する際は、必要なオプションを組み合わせて、特定のリソースに焦点を当てると良いでしょう。
- リアルタイムでの監視が可能なため、パフォーマンスのボトルネックを特定するのに役立ちます。
- スクリプトに組み込むことで、定期的なリソース監視を自動化することも可能です。