# Tailwind CSS

> A utility-first CSS framework packed with classes like `flex`, `pt-4`, `text-center` and `rotate-90` that can be composed to build any design, directly in your markup.


## Tailwind CSS VS Bootstrap

* [Tailwind CSS](https://tailwindcss.com/docs)
* [Bootstrap](https://getbootstrap.com/docs/5.0/getting-started/introduction/)

## Tailwind CSS 可以做到什麼

### 提供一套設計規範

### 響應式設計 Responsive Design

#### Mobile First

Before
```
// In CSS
@media (min-width: 768px) { ... }
@media (min-width: 1024px) { ... }
```

After
```
<!-- Width of 16 by default, 32 on medium screens, and 48 on large screens -->
<img class="w-16 md:w-32 lg:w-48" src="...">
```

### hover, active, focus 狀態

Before
```
```

After
```
```

[Example]

### Darkmode

Before
```
```

After
```
```

[Example]

## Tailwind CSS 客製化

VSCode extension
[Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)


---
## 真的覺得 Inline classes 很醜怎麼辦？

1. 組件化習慣
2. 善用 `@apply`

```
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
## 什麼情況下適合用 Tailwind CSS？

* 對 cSS 具熟悉度
* 完全沒有設計規範 VS 團隊有完善設計規範
* 有組件概念的專案

## 學習更多

官方文件
* [Tailwind CSS 中文技術文件](https://www.tailwindcss.cn/docs)

教學影片
* [Tailwind Labs](https://www.youtube.com/c/TailwindLabs/videos)
* [Adam Wathan aka Tailwind CSS creator's YouTube channel](https://www.youtube.com/c/AdamWathan/videos)

工具
* [官方組件庫 Tailwind UI](https://tailwindui.com/)
* [社群組件庫 Tailwind Components](https://tailwindcomponents.com/components)
