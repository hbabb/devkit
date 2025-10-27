
```JavaScript
const root = document.documentElement;
const baseSize = getComputedStyle(root).fontSize;
root.style.setProperty('--base-font-size', baseSize);
```
```sass
:root {
    --base-font-size: 16px;
}

@function rem($px) {
    @return calc(#{$px}px / var(---base-font-size) * 1rem);
}
```
