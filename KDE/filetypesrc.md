# Настройки приложений по умолчанию

Документация по управлению приложениями

Путь к конфигу: `~/.config/filetypesrc`
Путь к конфигу: `~/.config/mimeapps.list`

## Приложения по умолчанию

### Приложения - Приложения по умолчанию

![""](../img/20230720_163901.png "")

### Текстовый редактор

При изменении текстового редактора по умолчанию, на текстовый редактор kate,

в конфиги добавляются новые параметры.

В файл `~/.config/mimeapps.list` добавляются строки параметров

```ini
application/json=kde5-org.kde.kate.desktop;
application/x-docbook+xml=kde5-org.kde.kate.desktop;
application/x-yaml=kde5-org.kde.kate.desktop;
text/markdown=kde5-org.kde.kate.desktop;
text/plain=kde5-org.kde.kate.desktop;
text/x-cmake=kde5-org.kde.kate.desktop;
application/json=kde5-org.kde.kate.desktop;
application/x-docbook+xml=kde5-org.kde.kate.desktop;
application/x-yaml=kde5-org.kde.kate.desktop;
text/markdown=kde5-org.kde.kate.desktop;
text/plain=kde5-org.kde.kate.desktop;
text/x-cmake=kde5-org.kde.kate.desktop;
```

В файл `~/.config/filetypesrc` добавляются строки параметров


```ini
embed-application/json=false
embed-application/x-docbook+xml=false
embed-application/x-yaml=false
embed-text/markdown=false
embed-text/plain=false
embed-text/x-cmake=false
```
