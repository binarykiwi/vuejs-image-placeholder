# Vuejs Image Placeholder

> svg image placeholder

Creates a customisable svg image placeholder

## Install

```bash
npm install vuejs-image-placeholder
```

## Usage

All props are optional

Basic
```html
<image-placeholder
    :width="200"
    :height="200"
    :background-color="#ddd"
    :border-color="#000"
    :border-width="2"
    :show-ratio="true"
    :font-family="Tahoma, sans-serif"
    :font-color="#333"
    :font-size="18"
    :class="mycustomclass"
></image-placeholder>
```

By default the image shows the dimensions, using `showRatio` prop the ratio can displayed instead.
Alternatively you can provide your own text.

```html
<image-placeholder>My Custom Text</image-placeholder>
```


## Available props

|Prop              |Type    |Default  |Description|
|------------------|--------|---------|----------|
|width             |Number  |200      |Img width |
|height            |Number  |150      |Img height|
|backgroundColor   |String  |#ccc     |Background color|
|borderColor       |String  |#333     |Border color|
|borderWidth       |Number  |1        |Border width|
|showRatio         |Boolean |false    |Show image size in pixels or the proportion ratio|
|fontFamily        |String  |monospace|Font for the display text|
|fontColor         |String  |#333     |Display text color|
|fontSize          |Number  |14       |Display text size|
|class             |String  |         |Add a custom css classname like img-round, etc if you need|
