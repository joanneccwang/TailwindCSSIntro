# Tailwind CSS

> A utility-first CSS framework packed with classes like `flex`, `pt-4`, `text-center` and `rotate-90` that can be composed to build any design, directly in your markup.


## Tailwind CSS VS Bootstrap

| [Tailwind CSS](https://tailwindcss.com/docs) | [Bootstrap](https://getbootstrap.com/docs/5.0/getting-started/introduction/) |
|----------------------------------------------|------------------------------------------------------------------------------|
| Utility-first CSS framework                  | HTML, CSS, and JavaScript framework                                          |
| Predefined utility classes for CSS `p-4`, `rounded`, `bg-green-200` | Predefined UI components & utilities `btn`, `card`, `col-6`, `border`       |
| :thumbsup: For websites that need customization | :thumbsup: For responsive website prototypes |



## What can Tailwind CSS do?

### :white_check_mark: Provide a Design System
* Work within the constraints of a system
* Stay consistent with spacing, sizing, color choices ...
* Customize and build your own design system through a config file

### :white_check_mark: Responsive Design

* Mobile first breakpoint system
* Apply breakpoints by prefixing utility classes with the breakpoint name. e.g. `md:w-32`

#### Before
```css
// In CSS
@media (min-width: 768px) { ... }
@media (min-width: 1024px) { ... }
```

#### After
```html
<!-- Width of 16 by default, 32 on medium screens, and 48 on large screens -->
<img class="w-16 md:w-32 lg:w-48" src="...">
```

### :white_check_mark: Apply CSS states, like hover, active, focus

* Apply states by prefixing utility classes with the appropriate state variant. e.g. `hover:bg-purple-700`

#### Before
```html
<button class="btn">
  Hover me
</button>

<style>
.btn {
  background-color: red;
}
.btn:hover {
  backgorund-color: darkred;
}
</style>
```

#### After
```html
<button class="bg-red-500 hover:bg-red-700">
  Hover me
</button>
```

### :white_check_mark: Darkmode

#### Before
```
<div class="theme"></div>
<style>
.theme {
  background-color: white;
}
@media (prefers-color-scheme: dark) {
  theme {
    background-color: black;
  }
}
</style>
```

#### After
```
<div class="bg-white darkmode:bg-black"></div>
```

### :white_check_mark: Tiny in production

## Tailwind CSS Customization

Install this if you use VSCode :arrow_right: [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)

---
## Inline classes are too UGLY :weary:

1. Extract components
2. `@apply` exists! Use it well.

```html
<!-- Using utilities -->
<button class="py-2 px-4 font-semibold rounded-lg shadow-md text-white bg-green-500 hover:bg-green-700">
  Click me
</button>

<!-- Extracting classes using @apply -->
<button class="btn btn-green">
  Button
</button>

<style>
  .btn {
    @apply py-2 px-4 font-semibold rounded-lg shadow-md;
  }
  .btn-green {
    @apply text-white bg-green-500 hover:bg-green-700;
  }
</style>
```
--- 
## Should I use Tailwind CSS？

#### Personal
* If you're familiar with CSS
* If you love to build things on your own instead of using UI kit libraries

#### Project
* If you have no design system at all
* If you have a proper design system provided by your design team
* If your project is component based

---
## Learn More
Official Documentation
* [Tailwind CSS 中文技術文件](https://www.tailwindcss.cn/docs)

Tutorials
* [Tailwind Labs](https://www.youtube.com/c/TailwindLabs/videos)
* [Adam Wathan aka Tailwind CSS creator's YouTube channel](https://www.youtube.com/c/AdamWathan/videos)

Tools
* [Tailwind UI](https://tailwindui.com/)
* [Tailwind Components](https://tailwindcomponents.com/components)
