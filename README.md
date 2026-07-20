# infmt-cdn

Публичное зеркало **только собранного бандла** INFMT для раздачи через jsDelivr.
Здесь лежат исключительно продакшн-файлы `dist/` — исходники, тесты и история
находятся в приватном репозитории `gbplf221/infmt` (источник правды).

Файлы генерируются автоматически (Vite, `npm run build` в приватном репозитории)
и копируются сюда при выпуске версии. Вручную не редактировать.

## Подключение (блок T123 на Тильде)

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/gbplf221/infmt-cdn@v0.1.0/dist/infmt.min.css">
<div data-infmt-mode="demo"></div>
<script defer src="https://cdn.jsdelivr.net/gh/gbplf221/infmt-cdn@v0.1.0/dist/infmt.min.js"></script>
```

Версия фиксируется тегом (`@v0.1.0`) — jsDelivr кэширует каждый тег неизменно.

## Выпуск новой версии

В приватном репозитории `infmt`: `npm run build`. Затем скопировать
`dist/infmt.min.js` и `dist/infmt.min.css` сюда, закоммитить, поставить новый тег
(`v0.1.1`, `v0.2.0`, …) и запушить с тегами.
