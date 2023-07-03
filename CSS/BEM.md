# BEM
> 什么是BEM，BEM(全称Block-Element-Modifier)是一种CSS类的命名约定，它具有相当广泛的应用而且让我们码出来的CSS能够更加容易的阅读，理解以及度量方面非常有用

## BEM各代表什么
- Block(块)
块为最外层的标识，通常代表更高级别的抽象或组件
- Element(元素)
元素则为一个块内具体的元素，常用的有
> 表单元素 form form-item input select radio checkbox switch rate datePicker
导航元素 nav subnav menu tab
提示 alert message messageBox notification
数据展示 table process tree pagiantion
其他 button icon

- Modifier(修饰符)
modifier代表该块、元素对应不同状态的不同版本

>\-  中划线 ：仅作为连字符使用，表示某个块或者某个子元素的多单词之间的连接记号。
>__  双下划线：双下划线用来连接块和块的子元素
>_   单下划线：单下划线用来描述一个块或者块的子元素的一种状态

type-block__element_modifier

例如一下的网页元素
```html
<div>
  <button>按钮</button>
  <input/>
  <span>这是span标签</span>
  <div>test</div>
</div>
```
如果添加class
```html
<div class="page">
  <button class="page__button">按钮</button>
  <input class="page__input"/>
  <span class="page__span_default page__span_active">这是span标签</span>
</div>
```
