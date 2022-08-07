# Review CSS

## Property

- text-align
- color
- font-family

```html
<h1 style="text-align: center;">Review CSS</h1>
```

## Function

- rgb()
- url()

```html
<h1 style="color: rgb(255,0,0);">Review CSS</h1>
```

## Selector

- Universal: *
- Type: h1
- Class: .classname
- ID: #id
- Attribute: [attribute=value]
- Group: a, b
- Descendant combinator: a b
- Child combinator: a > b

```css
h1, p {
    color: #ff0000;
}

table > tr {
    text-align: center;
}

.text-center {
    text-align: center;
}

[class=text-center] {
    text-align: center;
}
```

## At-rules (@)

- @font-face
- @import
- @media

```css
@font-face {
    font-family: 'Nome A';
    src: url(https://...);
}
```

## Media Query

```html
<link rel="stylesheet" href="print.css" media="print">
```

```css
h1 {
    text-align: center;
}

@media screen and (max-width: 425px) {
    h1 {
        text-align: justify;
    }
}

@media print {
    #menu {
        display: none;
    }
}
```

## Cascate Style Sheet

- Important
- Specificity
- Local
