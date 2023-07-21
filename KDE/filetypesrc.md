# Настройки приложений по умолчанию

Документация по управлению приложениями

Путь к конфигу: `~/.config/filetypesrc`
Путь к конфигу: `~/.config/mimeapps.list`

## Приложения по умолчанию

### Приложения - Приложения по умолчанию

![""](../img/20230720_163901.png "")

### Текстовый редактор

При выборе текстовым редактором по умолчанию, текстового редактора kate,

в конфиги добавляются новые параметры.


В созданный файл `~/.config/filetypesrc` добавляются строки параметров

```ini
[EmbedSettings]
embed-application/json=false
embed-application/x-docbook+xml=false
embed-application/x-yaml=false
embed-text/markdown=false
embed-text/plain=false
embed-text/x-cmake=false
```

В созданный файл `~/.config/mimeapps.list` добавляются строки параметров

```ini
[Added Associations]
application/json=kde5-org.kde.kate.desktop;
application/x-docbook+xml=kde5-org.kde.kate.desktop;
application/x-yaml=kde5-org.kde.kate.desktop;
text/markdown=kde5-org.kde.kate.desktop;
text/plain=kde5-org.kde.kate.desktop;
text/x-cmake=kde5-org.kde.kate.desktop;
```

```ini
[Default Applications]
application/json=kde5-org.kde.kate.desktop;
application/x-docbook+xml=kde5-org.kde.kate.desktop;
application/x-yaml=kde5-org.kde.kate.desktop;
text/markdown=kde5-org.kde.kate.desktop;
text/plain=kde5-org.kde.kate.desktop;
text/x-cmake=kde5-org.kde.kate.desktop;
```

При выборе текстовым редактором по умолчанию, текстового редактора kwrite,

в конфиге заменяются параметры текстового редактора на новые значения.

Заменяется приложение по умолчанию, и добавляется приложение для ассоциации файлов.

В файл `~/.config/mimeapps.list` заменяяются строки параметров, на

```ini
[Added Associations]
application/json=kde5-org.kde.kwrite.desktop;kde5-org.kde.kate.desktop;
application/x-docbook+xml=kde5-org.kde.kwrite.desktop;kde5-org.kde.kate.desktop;
application/x-yaml=kde5-org.kde.kwrite.desktop;kde5-org.kde.kate.desktop;
text/markdown=kde5-org.kde.kwrite.desktop;kde5-org.kde.kate.desktop;
text/plain=kde5-org.kde.kwrite.desktop;kde5-org.kde.kate.desktop;
text/x-cmake=kde5-org.kde.kwrite.desktop;kde5-org.kde.kate.desktop;
```

```ini
[Default Applications]
application/json=kde5-org.kde.kwrite.desktop;
application/x-docbook+xml=kde5-org.kde.kwrite.desktop;
application/x-yaml=kde5-org.kde.kwrite.desktop;
text/markdown=kde5-org.kde.kwrite.desktop;
text/plain=kde5-org.kde.kwrite.desktop;
text/x-cmake=kde5-org.kde.kwrite.desktop;
```

### Почтовый клиент

При выборе почтовым клиентом по умолчанию, почтового клиента kmail,

в конфиги добавляются новые параметры.

В файл `~/.config/filetypesrc` добавляются строки параметров

```ini
[EmbedSettings]
embed-x-scheme-handler/mailto=false
```

В файл `~/.config/mimeapps.list` добавляются строки параметров

```ini
[Added Associations]
x-scheme-handler/mailto=kde5-org.kde.kmail2.desktop;
```

```ini
[Default Applications]
x-scheme-handler/mailto=kde5-org.kde.kmail2.desktop;
```

При выборе почтовым клиентом по умолчанию, почтового клиента Thunderbird,

в конфиге заменяются параметры почтового клиента на новые значения.

Заменяется приложение по умолчанию, и добавляется приложение для ассоциации файлов.

В файл `~/.config/mimeapps.list` добавляются строки параметров

```ini
[Added Associations]
x-scheme-handler/mailto=thunderbird.desktop;kde5-org.kde.kmail2.desktop;
```

```ini
[Default Applications]
x-scheme-handler/mailto=thunderbird.desktop;
```
