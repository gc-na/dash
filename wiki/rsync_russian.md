# [Русский] Debian Almquist Shell (dash) rsync Использование: Синхронизация файлов и каталогов

## Обзор
Команда `rsync` используется для синхронизации файлов и каталогов между локальными и удалёнными системами. Она эффективна и позволяет передавать только изменённые части файлов, что значительно экономит время и ресурсы.

## Использование
Основной синтаксис команды выглядит следующим образом:

```bash
rsync [options] [arguments]
```

## Общие параметры
- `-a` : Архивный режим, который сохраняет права доступа, временные метки и символические ссылки.
- `-v` : Подробный режим, выводит информацию о процессе передачи.
- `-z` : Сжимает данные во время передачи для уменьшения объёма передаваемых данных.
- `-r` : Рекурсивно копирует каталоги.
- `--delete` : Удаляет файлы в целевом каталоге, которые отсутствуют в исходном каталоге.

## Общие примеры
1. Синхронизация локальной директории с удалённой:

```bash
rsync -av /path/to/local/dir/ user@remote:/path/to/remote/dir/
```

2. Синхронизация с удалённым сервером с использованием сжатия:

```bash
rsync -avz user@remote:/path/to/remote/dir/ /path/to/local/dir/
```

3. Синхронизация с удалением отсутствующих файлов в целевой директории:

```bash
rsync -av --delete /path/to/local/dir/ user@remote:/path/to/remote/dir/
```

4. Синхронизация с выводом подробной информации:

```bash
rsync -av --progress /path/to/local/file user@remote:/path/to/remote/file
```

## Советы
- Используйте флаг `-n` (или `--dry-run`), чтобы сначала просмотреть, какие изменения будут внесены, не выполняя фактическую синхронизацию.
- Регулярно проверяйте права доступа и владельцев файлов, чтобы избежать проблем с доступом после синхронизации.
- Рассмотрите возможность использования SSH для безопасной передачи данных, добавив `-e ssh` в команду.