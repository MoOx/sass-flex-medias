# Flex Medias

## [DEPRECATED, consider [SUIT flex embed](https://github.com/suitcss/components-flex-embed/)]

> Flexible responsive fixed ratio medias to avoid browsers reflow.

Some helpers for responsive, intrinsic ratio medias (video, iframe, objects, images...). It also avoid browsers reflow.

![Fonzie approved](https://dl.dropbox.com/u/14108185/Pictures/fonzie.jpg)

---

**NOT TESTED & NOT PUBLISHED ON FONZIE YET**

## Installation

```
fonzie install flex-medias
```

## Usage

```scss
@import "flex-medias";
```

### BEM style

```scss
$flex-media-selector: '.flex-media';
$flex-media-ratios: "3-1" 3, "16-9" 16/9, "4-3" 4/3, "1-1" 1;
@include flex-medias();
```

```html
<figure class="flex-media flex-media--16-9">
    <a href="#zoomOrWhatever">
        <img class="flex-media__item" src="..." alt="" />
    </a>
</figure>
```

### `@extend` style

```scss
@import "flex-media";
$flex-media-ratios: "3-1" 3, "16-9" 16/9, "4-3" 4/3, "1-1" 1;
@include flex-medias();
```

```html
<figure class="flex-media--16-9"><!-- flex-media--16-9 inherit from flex-media using @extend -->
    <a href="#zoomOrWhatever">
        <img class="flex-media__item" src="..." alt="" />
    </a>
</figure>
```

---

## License

Copyright (c) 2013 Maxime Thirouin

Released under [MIT Licence](http://moox.mit-license.org/)
