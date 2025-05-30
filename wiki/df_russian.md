# [Русский] Debian Almquist Shell (dash) df Использование: отображение информации о файловой системе

## Обзор
Команда `df` используется для отображения информации о доступном и используемом пространстве на файловых системах. Она предоставляет пользователю представление о том, сколько места занято и сколько доступно на каждом подключенном разделе.

## Использование
Основной синтаксис команды выглядит следующим образом:
```
df [опции] [аргументы]
```

## Общие опции
- `-h` — отображает размеры в удобочитаемом формате (например, КБ, МБ).
- `-T` — показывает тип файловой системы.
- `-a` — включает в вывод файловые системы с нулевым размером.
- `-i` — отображает информацию о индексных узлах вместо блоков.

## Общие примеры
1. Отобразить информацию о всех файловых системах:
   ```sh
   df
   ```

2. Отобразить информацию в удобочитаемом формате:
   ```sh
   df -h
   ```

3. Показать тип файловой системы для каждого раздела:
   ```sh
   df -T
   ```

4. Отобразить информацию о файловых системах с нулевым размером:
   ```sh
   df -a
   ```

5. Показать информацию о индексных узлах:
   ```sh
   df -i
   ```

## Советы
- Используйте опцию `-h`, чтобы быстро получить информацию о свободном месте в понятном формате.
- Регулярно проверяйте использование дискового пространства, чтобы избежать переполнения файловых систем.
- Комбинируйте опции для получения более детальной информации, например, `df -hT` для отображения и размера, и типа файловой системы.