# SCSS theme mixins

scss mixins for create theme styles in project

```scss
@import "theme/mixin-theme";

.example {
    @include set-color-theme(color, clr-invert);
    @include set-color-theme-sub(background-color, clr-primary, '', '!important');
}
``` 

it will generate to

```css

.example {
    color: #e0e0e0;
    background-color: #212121 !important;
}

.theme-light .example {
    color: #212121;
}

.theme-light .example {
    background-color: #e0e0e0 !important;
}

```

 licence: MIT, dudiq 2018
