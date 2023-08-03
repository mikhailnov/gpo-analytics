# Настройка отображения миниатюр в dolphin

Документация по настройкам миниатюр в dolphin

Путь к конфигу: `~/.config/dolphinrc`

## Миниатюты

### Меню Dolphin - Настройка - Настроить Dolphin... - Главное - Миниатюры

![""](../img/20230803_170734.png "")

При включении отображения всех миниатюр, в файл конфига добавляется параметр

```ini
[PreviewSettings]
Plugins=appimagethumbnail,mltpreview,ffmpegthumbs,opendocumentthumbnail,kraorathumbnail,audiothumbnail,imagethumbnail,exrthumbnail,jpegthumbnail,windowsimagethumbnail,svgthumbnail,windowsexethumbnail,comicbookthumbnail,directorythumbnail,textthumbnail,blenderthumbnail,djvuthumbnail,gsthumbnail,cursorthumbnail,fontthumbnail,rawthumbnail,ebookthumbnail,mobithumbnail
```

Для отключения отображения любых миниатюр, нужно из секции удалить все движки миниатюр,

приведя запись секции к такому виду.

```ini
[PreviewSettings]
Plugins=
```

### Блокировка параметров

Для запрета пользователю производить изменение отображения миниатюр,

с полным запретом отображения миниатюр, в файле `/etc/xdg/dolphinrc`

блокируется изменение параметров, символами блокировки строки параметра `[$i]`,

и отображения миниатюр становятся недоступны для изменения:

##### Блокировка строки параметра

```ini
[PreviewSettings]
Plugins[$i]=
```

##### Блокировка секции

```ini
[PreviewSettings][$i]
Plugins=
```
