# 教学内容

## 1. Emmit 语法

> 前端神级插件 Emmit: 让写 html 的速度飞起来, 主流编辑器大多已内置,如 vscode

| 用途 | 标记                                   | 描述                |
| ---- | -------------------------------------- | ------------------- |
| 属性 | `#`id, `.`class,`[...]`属性            | 默认元素`<div>`     |
| 内容 | `{...}`标签或属性值                    | 纯文本,不能嵌套标签 |
| 层级 | `+`同级, `>`: 父子                     | `>`支持多级         |
| 重复 | `*`n , 常用于层级结构中                | n:必须是正整数      |
| 序号 | `$`默认升序,`$@-5`反序,`$@-5`指定反序  | n:必须是正整数      |
| 分组 | `(...)`内部可放置任意类型的 emmit 标记 | emmit 结构更清晰    |

## 2. 元素属性

| 类型       | 描述                                                           |
| ---------- | -------------------------------------------------------------- |
| 通用属性   | id,class,style,title 等,几乎可用于所有元素                     |
| 预置属性   | 除通用属性外,w3c 还为每个不同功能的元预置一些属性,来区别他们   |
| 事件属性   | 它是预置属性的一个子集,根据元素特征,所支持的事件属性也各不相同 |
| 自定义属性 | 为方便编程,由用户为元素添加的属性,以`data-`为前缀              |

## 3. 常用元素

| 类型         | 描述                                                               |
| ------------ | ------------------------------------------------------------------ |
| 布局元素     | `<header><footer><main><aside><article><nav><section><h1...><div>` |
| 文本元素     | `<span><p><time><code><strong><q>...`                              |
| 链接元素     | `<a href="xxx" target="_self/_blank/name">`                        |
| 图像元素     | `<figure><figcaption><img src="xxx" alt="xxx"><picture><source>`   |
| 列表元素     | 无序`<ul>+<li>` , 有序`<ol>+<li>`, 自定义`<dl>+<dt>+<dd>`          |
| 表格元素     | `<table><caption><thead><tbody><tfoot><tr><td><col>...`            |
| **表单元素** | `<form><label><input><datalist><select><textarea><button>`         |
| 内联框架     | `<iframe src="xxx" name="xxx">`,常用于后台布局或前端跨域           |
| 音/视频      | `<video src="xxx" controls><audio src="xxx" controls>`             |

> 更多 html 元素: <https://developer.mozilla.org/zh-CN/docs/Web/HTML>
