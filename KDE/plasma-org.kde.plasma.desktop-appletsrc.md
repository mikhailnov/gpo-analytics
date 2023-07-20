# Общие настройки в профиле пользователя

Документация по plasma-org.kde.plasma.desktop-appletsrc

Путь к конфигу: `~/.config/plasma-org.kde.plasma.desktop-appletsrc`

### Расположение значков на рабочем столе

Если в файле ~/.config/plasma-org.kde.plasma.desktop-appletsrc

В секцию

```ini
[Containments][40][General]
ToolBoxButtonState=topcenter
ToolBoxButtonX=748
```

добавить параметр `arrangement=1`, запись параметра вот такого вида

```ini
[Containments][40][General]
ToolBoxButtonState=topcenter
ToolBoxButtonX=748
arrangement=1
```

будет установлено размещение значков `Сверху вниз`

Если из этой секции удалить параметр `arrangement=1`,

сделать запись парамера вот такого вида


```ini
[Containments][40][General]
ToolBoxButtonState=topcenter
ToolBoxButtonX=748
```

будет установлено размещение значков `Слева направо`

