---
id: 587d7faa367417b2b2512bd2
title: 给 D3 元素添加标签
challengeType: 6
forumTopicId: 301476
---

# --description--

D3 允许使用 SVG 的 `text` 元素给图形元素贴标签，例如给条形图中的各组都贴上标签。

和 `rect` 元素类似，`text` 元素也需要 `x` 和 `y` 属性来指定其放置在 SVG 画布上的位置，它也需要能够获取数据来显示数据值。

关于如何给组贴标签，D3 给了你很高的控制权。

# --instructions--

编辑器中的代码已经将数据绑定到每个新的 `text` 元素。首先，在 `svg` 中添加 `text` 节点。然后，添加 `x` 和 `y` 坐标属性，除了 `text` 的 `y` 值应该使标签比组的高 `y` 3 个单位，其余值的计算方法应该和 `rect` 中计算方法一样。最后，用 D3 的 `text()` 方法将标签的文本设置为和数据点相等的值。

**提示**  
关于标签比组高，想一想 `text` 的 `y` 值应该比组的 `y` 值大 3 还是小 3。

# --hints--

第一个 `text` 元素应该有一个值为 12 的标签并且 `y` 值为 61。

```js
assert($('text').eq(0).text() == '12' && $('text').eq(0).attr('y') == '61');
```

第二个 `text` 元素应该有一个值为 31 的标签并且 `y` 值为 4。

```js
assert($('text').eq(1).text() == '31' && $('text').eq(1).attr('y') == '4');
```

第三个 `text` 元素应该有一个值为 22 的标签并且 `y` 值为 31。

```js
assert($('text').eq(2).text() == '22' && $('text').eq(2).attr('y') == '31');
```

第四个 `text` 元素应该有一个值为 17 的标签并且 `y` 值为 46。

```js
assert($('text').eq(3).text() == '17' && $('text').eq(3).attr('y') == '46');
```

第五个 `text` 元素应该有一个值为 25 的标签并且 `y` 值为 22。

```js
assert($('text').eq(4).text() == '25' && $('text').eq(4).attr('y') == '22');
```

第六个 `text` 元素应该有一个值为 18 的标签并且 `y` 值为 43。

```js
assert($('text').eq(5).text() == '18' && $('text').eq(5).attr('y') == '43');
```

第七个 `text` 元素应该有一个值为 29 的标签并且 `y` 值为 10。

```js
assert($('text').eq(6).text() == '29' && $('text').eq(6).attr('y') == '10');
```

第八个 `text` 元素应该有一个值为 14 的标签并且 `y` 值为 55。

```js
assert($('text').eq(7).text() == '14' && $('text').eq(7).attr('y') == '55');
```

第九个 `text` 元素应该有一个值为 9 的标签并且 `y` 值为 70。

```js
assert($('text').eq(8).text() == '9' && $('text').eq(8).attr('y') == '70');
```

# --solutions--

