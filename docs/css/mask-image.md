# mask-image

Свойство **`mask-image`** устанавливает изображение, которое используется как слой маски для элемента.

## Синтаксис

```css
/* Keyword value */
mask-image: none;

/* <mask-source> value */
mask-image: url('masks.svg#mask1');

/* <image> values */
mask-image: linear-gradient(rgba(0, 0, 0, 1), transparent);
mask-image: image(url('mask.png'), skyblue);

/* Multiple values */
mask-image: image(url('mask.png'), skyblue), linear-gradient(rgba(0, 0, 0, 1), transparent);

/* Global values */
mask-image: inherit;
mask-image: initial;
mask-image: unset;
```

## Значения

- `none` -- это ключевое слово интерпретируется как прозрачный слой черного изображения.
- `<mask-source>` -- ссфлка `<url>` на `<mask>` или изображение.
- `<image>` -- изображение, используемое в качестве слоя маски.

Значение по-умолчанию:

```css
mask-image: none;
```

Применяется к:

## Спецификации

- [CSS Masking Module Level 1](https://drafts.fxtf.org/css-masking-1/#the-mask-image)

## Поддержка браузерами

<p class="ciu_embed" data-feature="css-masks" data-periods="future_1,current,past_1,past_2">
  <a href="http://caniuse.com/#feat=css-masks">Can I Use css-masks?</a> Data on support for the css-masks feature across the major browsers from caniuse.com.
</p>

## Описание и примеры

```html tab="HTML"
<div id="masked"></div>
```

```css tab="CSS"
#masked {
  width: 100px;
  height: 100px;
  background-color: #8cffa0;
  -webkit-mask-image: url('https://mdn.mozillademos.org/files/12676/star.svg');
  mask-image: url('https://mdn.mozillademos.org/files/12676/star.svg');
}
```