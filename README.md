# MysticLollipopRP

Публичный resource pack для плагина MysticLollipop (Minecraft **1.21.11**).

## Установка на сервере

В `server.properties`:

```properties
resource-pack=https://raw.githubusercontent.com/abibaokak/MysticLollipopRP/main/MysticLollipopRP.zip
resource-pack-sha1=9f6aed021b183e3aaf71453be4ea38c78339e13f
require-resource-pack=true
```

После изменения перезапустите сервер. Если на нём уже настроен другой resource pack, замените его URL и SHA1 указанными выше — иначе клиент будет грузить старый пак и леденец не отобразится.

## Что исправлено

В предыдущей версии `pack.mcmeta` использовал `min_format: 75.0` / `max_format: 75.0`. С 1.21.9 эти поля должны быть целым числом или массивом `[75, 0]`; float `75.0` приводит к отклонению пака. Сейчас используется `[75, 0]`.

Пак меняет только `minecraft:netherite_sword` при `custom_model_data: 3001`. Обычные незеритовые мечи остаются без изменений.

Текстура: `assets/mysticlollipop/textures/item/mystic_lollipop.png`, 16×16, без перекрашивания.
