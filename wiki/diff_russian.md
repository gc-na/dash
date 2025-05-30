# [Русский] Debian Almquist Shell (dash) diff <Использование эквивалента на русском языке>: Сравнение файлов

## Обзор
Команда `diff` используется для сравнения содержимого двух файлов или каталогов. Она показывает различия между ними, что позволяет пользователям видеть, какие строки были добавлены, удалены или изменены.

## Использование
Основной синтаксис команды выглядит следующим образом:

```bash
diff [опции] [аргументы]
```

## Общие опции
- `-u` — выводит различия в унифицированном формате, который удобнее для чтения.
- `-i` — игнорирует регистр при сравнении.
- `-w` — игнорирует все пробелы.
- `-r` — рекурсивно сравнивает каталоги.

## Общие примеры
1. Сравнение двух текстовых файлов:
   ```bash
   diff file1.txt file2.txt
   ```

2. Сравнение двух файлов с игнорированием регистра:
   ```bash
   diff -i file1.txt file2.txt
   ```

3. Вывод различий в унифицированном формате:
   ```bash
   diff -u file1.txt file2.txt
   ```

4. Рекурсивное сравнение двух каталогов:
   ```bash
   diff -r dir1/ dir2/
   ```

## Советы
- Используйте опцию `-u` для более понятного вывода, особенно если вы планируете делиться результатами с другими.
- При работе с большими файлами или каталогами, рассмотрите возможность использования `diff` в сочетании с `less` для удобного просмотра:
  ```bash
  diff -u file1.txt file2.txt | less
  ```
- Регулярно проверяйте различия в конфигурационных файлах, чтобы отслеживать изменения и избегать ошибок.