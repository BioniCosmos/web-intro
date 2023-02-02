---
theme: seriph
background: https://images.unsplash.com/photo-1451187580459-43490279c0fa
---

# Web

从入门到……？

---

# 什么是 Web？

World Wide Web，万维网

- Tim Berners-Lee
- 开放
- HTTP
- HTML、CSS、JavaScript
- 浏览器
- ……

---

# Web 技术能做什么？

- 网页
- 小程序
- 游戏
- ……

---
layout: section
---

# HTML

---

# 什么是 HTML？

HyperText Markup Language，超文本标记语言

- 一种用来结构化 Web 网页及其内容的标记语言。网页内容可以是：一组段落、一个重点信息列表、也可以含有图片和数据表。
- 不是一门编程语言，而是一种用于定义内容结构的标记语言。
- 由一系列的元素组成，这些元素可以用来包围不同部分的内容，使其以某种方式呈现或者工作。一对标签可以为一段文字或者一张图片添加超链接，将文字设置为斜体，改变字号，等等。

---

# 样例

```html {all|1|2-11|3-6|7-10}
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>测试页面</title>
  </head>
  <body>
    <img src="images/web.png">
    <p id="greeting">你好！</p>
  </body>
</html>
```

---

# HTML 元素

<div class="flex justify-center items-center h-3/4">

![](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-small.png)

</div>

---
layout: center
---

![](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-attribute-small.png)

---
layout: section
---

# CSS

---

# CSS 是什么？

Cascading Style Sheets，层叠样式表

- 为网页添加样式的代码。
- 设置文本颜色，调整元素位置，更改背景。
- 不是编程语言，也不是标记语言，而是一门样式表语言。

---

# CSS 规则集

<div>

![](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics/css-declaration-small.png)

</div>

<style>
  img {
    @apply transform scale-75
  }
</style>

---

# 选择器

| 选择器名称 | 选择的内容               | 示例                                                              |
| ---------- | ------------------------ | ----------------------------------------------------------------- |
| 元素选择器 | 所有指定类型的 HTML 元素 | `p` 选择 `<p>`                                                    |
| ID 选择器  | 具有特定 ID 的元素       | `#my-id` 选择 `<p id="my-id">`                                    |
| 类选择器   | 具有特定类的元素         | `.my-class` 选择 `<p class="my-class">` 和 `<a class="my-class">` |
| 属性选择器 | 拥有特定属性的元素       | `img[src]` 选择 `<img src="myimage.png">` 而不是 `<img>`          |
| 伪类选择器 | 特定状态下的特定元素     | `a:hover` 仅在鼠标指针悬停在链接上时选择 `<a>`                    |

---
layout: image-right
image: https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics/boxes.jpg
---

# CSS 核心思想

- 层叠
- 继承
- 盒模型

---
layout: section
---

# JavaScript

---

# JavaScript 是什么？

- 一门完备的编程语言 
- 与 Java **没有**关系！（蹭热度）
- 可为网站添加交互功能。（例如：游戏、动态样式、动画以及在按下按钮或收到表单数据时做出的响应等）
- 浏览器 to 全平台（Node、Deno）

---
clicks: 5
---

# 语法横向对比

<div class="flex gap-8">
  <div class="w-full basis-1/2">

  ## C

  <v-click at="1">

  ```c
  printf("Hello, world!\n");
  ```

  </v-click>
  <v-click at="2">
  
  ```c
  const double pi = 3.14;
  int count = 0;
  ```

  </v-click>
  <v-click at="3">

  ```c
  if (count > 0) {
    return true;
  } else {
    return false;
  }
  ```

  </v-click>
  <v-click at="4">

  ```c
  for (int i = 0; i < 5; i++) {
    count++;
  }
  ```

  </v-click>
  <v-click at="5">

  ```c
  double calcCircleArea(double radius) {
    return pi * radius * radius;
  }
  ```

  </v-click>
  </div>
  <div class="w-full basis-1/2">
  
  ## JavaScript

  <v-click at="1">

  ```javascript
  console.log('Hello, world!')
  ```

  </v-click>
  <v-click at="2">

  ```javascript
  const pi = 3.14
  let count = 0
  ```

  </v-click>
  <v-click at="3">

  ```javascript
  if (count > 0) {
    return true
  } else {
    return false
  }
  ```

  </v-click>
  <v-click at="4">

  ```javascript
  for (let i = 0; i < 5; i++) {
    count++
  }
  ```

  </v-click>
  <v-click at="5">

  ```javascript
  function calcCircleArea(radius) {
    return pi * radius * radius
  }
  ```

  </v-click>
  </div>
</div>

---
layout: quote
---

Atwood’s Law:

# “Any application that can be written in JavaScript, will eventually be written in JavaScript.”

JavaScript 是万能语言。

---

# 更多细节

- 跨浏览器兼容性（Cross-browser compatibility）：不同种类，从新到旧
- 响应式网页设计（Responsive Web design：根据窗口大小自适应
- 性能（Performance）：快速、流畅、高效
- 无障碍（Accessibility）：残障人士
- 国际化（Internationalization）：多语言、地区
- 隐私与安全（Privacy & Security）：合理地处理数据

---
layout: none
---

<div class="h-full w-full flex bg-[#e0e0e0] justify-center items-center">
  <div id="outer">
    <div class="transform scale-75 flex flex-col justify-center items-center p-10">
      <img class="rounded-full w-32 h-32" src="https://cdn.moecm.com/avatar.jpg">
      <div class="text-3xl font-bold mt-8 mb-2">Daniel</div>
      <div>Blog: <a href="https://moecm.com/">https://moecm.com</a></div>
      <div>Email: <a href="mailto:daniel@moecm.com">daniel@moecm.com</a></div>
    </div>
  </div>
</div>

<style>
  #outer {
    border-radius: 50px;
    background: #e0e0e0;
    box-shadow: 20px 20px 60px #bebebe,
                -20px -20px 60px #ffffff;
  }
</style>
