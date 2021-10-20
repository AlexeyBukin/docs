# Изображения и файлы

## Вставить изображение {#add-image}

Чтобы добавить на страницу изображение, используйте разметку:

```
![Альтернативный текст](адрес изображения)
```

{% note info %}

Если вы вставите в текст страницы ссылку на изображение без элементов разметки, на странице отобразится изображение без альтернативного текста.

{% endnote %}

Разметка | Результат
--- | ---
`![Лого]({{ yandex-logo-link }})` | ![](../../_assets/wiki/logo95x37x8.png)

### Задать размер изображения {#img-size}

Задайте размер изображения на странице в пикселях:

```
<ширина>x<высота>:<ссылка на рисунок>
```

{% note info %}

Изображение масштабируется пропорционально, поэтому значение высоты можно задать приблизительно. Например, рисунок с такой разметкой будет отображаться правильно: `300x0:<ссылка на рисунок>`.

{% endnote %}

Разметка | Результат
--- | ---
`no-highlight 60x20:{{ yandex-logo-link }}` | ![](../../_assets/wiki/resize-pic.png)

### Вставить ссылку на скачивание изображения {#download-link}

Используйте обычную разметку ссылки:

```
[текст ссылки](адрес изображения)
```

Разметка | Результат
--- | ---
`[Логотип Яндекса]({{ yandex-logo-link }})` | [Логотип Яндекса]({{ yandex-logo-link }})

### Сделать изображение ссылкой {#img-link}

Вы можете сделать изображение ссылкой, чтобы при нажатии на изображение открывалась страница или файл. Для этого в элемент разметки ссылки вместо текста [вставьте изображение](#add-image):

```
[![Альтернативный текст](адрес изображения)](адрес ссылки)
```

Разметка | Результат
--- | ---
`[![Лого]({{ yandex-logo-link }})]({{ link-yandex }})` | [![Лого](../../_assets/wiki/logo95x37x8.png)]({{ link-yandex }})

## Вставить видео {#video}

Чтобы добавить на страницу видео, используйте [динамический блок `not_var{{iframe}}`](../actions/iframe.md). Он позволяет вставлять видео из внешних источников, таких как Vimeo или Youtube.

## Вставить ссылку на файл {#file-ref}

Разместите ссылку на файл в тексте страницы одним из способов:

Разметка | Результат
--- | ---
`http://адрес-файла` | [http://адрес-файла](http://адрес-файла)
`[текст ссылки](http://адрес-файла)` | [текст ссылки](http://адрес-файла)