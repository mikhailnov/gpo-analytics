# Настройка курсоров мыши

Документация по настройкам курсоров мыши

Путь к конфигу: `~/.config/kcminputrc`

## Курсоры мыши

### Внешний вид - Курсоры мыши

![""](../img/20230706_124734.png "")

Используются темы курсоров, доступные в `/usr/share/icons`

Допустимые значения параметра:

#### Breeze

```ini
[Mouse]
cursorTheme=breeze_cursors
```

#### Breeze, светлый вариант

```ini
[Mouse]
cursorTheme=Breeze_Snow
```

#### Wonderland

```ini
[Mouse]
cursorTheme=wonderland
```

### Блокировка параметров

Для запрета пользователю производить изменение курсоров мыши, в файле `/etc/xdg/kcminputrc`

блокируется изменение параметров, символами блокировки строки параметра `[$i]`, и курсороы мыши становятся

недоступны для изменения:

### Блокировка самой темы

#### Breeze

```ini
[Mouse]
cursorTheme[$i]=breeze_cursors
```

#### Breeze, светлый вариант

```ini
[Mouse]
cursorTheme[$i]=Breeze_Snow
```

### Блокировка группы

#### Wonderland

```ini
[Mouse][$i]
cursorTheme=wonderland
```

Если в файле `/etc/xdg/kcminputrc` параметры не заблокированы

символами блокировки строки параметра `[$i]`, то будет использоваться

тема курсоров мыши из темы оформления рабочей среды, заданной в файле

`/etc/xdg/kdeglobals`, из настроек по умолчанию для этой темы, заданных в файле

/usr/share/plasma/look-and-feel/`«оформление рабочей среды»`/contents/defaults

Параметры из файла `/etc/xdg/kdeglobals` имеют приоритет выше, чем у файла `/etc/xdg/kcminputrc`

Если в файле

/usr/share/plasma/look-and-feel/`«оформление рабочей среды»`/contents/defaults

не задана тема курсоров мыши, как, например, в теме оформления рабочей среды `org.kde.rosalight.desktop`,

то будет использоваться тема курсоров из файла `/etc/xdg/kcminputrc`
