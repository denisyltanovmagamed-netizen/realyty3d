# realty3d

Статический мобильный сайт-каталог недвижимости с интерактивным 3D-просмотром квартир.
Один HTML-файл (`index.html`), без сервера, без базы данных, без Node.js/npm.

## Структура

```
realty3d/
├── index.html                                 ← весь сайт: HTML+CSS+JS в одном файле
└── assets/
    ├── images/
    │   ├── profile.jpg                         ← фото риелтора (главная страница)
    │   ├── developments/
    │   │   └── zhk-moskovskiy/
    │   │       └── cover.jpg                   ← обложка ЖК "Московский"
    │   └── moskovskiy-001/                     ← сюда класть фото конкретной квартиры (1.jpg, 2.jpg...)
    └── models/
        └── moskovskiy-001/                     ← сюда класть .glb модель квартиры (model.glb)
```

## Как добавить новый ЖК или новую квартиру

Открой `index.html`, найди в нём массивы `DEVELOPMENTS` и `OBJECTS` — инструкция
по добавлению прямо в комментариях над ними.

## Публикация

GitHub → Settings → Pages → Source: ветка `main`, папка `/ (root)`.
Ссылка появится вида `https://<логин>.github.io/realty3d/`.
