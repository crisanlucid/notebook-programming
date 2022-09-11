#Steps how to organize SASS files

##links:

Design

1. [link 1](<https://www.figma.com/file/dx7FPC2YajKFAdTW9D1jAZ/Material-Design-Theme-Kit-(Copy)?node-id=0%3A1950>)

1. [link 2](https://www.figma.com/file/EX8VxcTtAatzI2PBLb361g/designsystems.engineering?node-id=99%3A0)

Repo:

1. [repo](https://github.com/bahdcoder/ds.e)

### Css Architecture Checklist

- Organised - fixed code structure

- No specificity issues

- Atomic design principles

- Easy to understand (comments, variables)
- Fully customizable / themeable

- Reusable across teams / projects

### Define System Variables

### Define Colors

### Define Typography

### Define mixins

### Global root and css reset

### Setup stylelint and prettier

### Setup husky and pre-commit hooks

### Compile from SCSS into CSS

file: src/scripts/build.js

```
yarn build
```

### CSS - Responsive Typography

using rem instead of px
using clamp() to have a responsive font resize over media queries
using CSS variable to change in one place font-sizes

```
$h-1-font-size: var(--h1-font-size, $h-1) !default;

:root {
   --h1-font-size: 2rem;
   --h1-font-size-xl: clamp(3.5rem, 12vw + 1rem, 12rem);//(min, adjust , maxim)
}
```

### Size types

- rem - root element`s font-size, relative length units
- em - font size parent, relative length units
- vw - view port width
- vh - view port height

notice: choosing vw, vh will not zoom

### how to reuse in many places font-size

1.

```
:root {
   --h1-font-size: 2rem;
   --h1-font-size-xl: clamp(3.5rem, 12vw + 1rem, 12rem);//(min, adjust , maxim)
}

```

2.

```
$h-1-font-size: var(--h1-font-size-xl, $h-1) !default;
```

3.

```
h1 {
    font-size: $h-1-font-size
}

@media (min-width: 40em) {
    :root {
        --h1-font-size-xl: 3rem;
    }
}
```
