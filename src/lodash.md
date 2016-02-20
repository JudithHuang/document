#lodash doc

ref: https://lodash.com/docs

## Array

### _.chunk(array, [size=1])

- 创建一个新的数组, 将数组分成长度为size的多个数组块, 如果不能均匀分割的话, 将剩余的元素放入到最后一个数组中

- example

```js
_.chunk(['a', 'b', 'c', 'd'], 2);
// => [['a', 'b'], ['c', 'd']]

_.chunk(['a', 'b', 'c', 'd'], 3);
// => [['a', 'b', 'c'], ['d']]
```

### _.compact(array)

- 移除数组中值为`false`, `null`, `0`, `""`, `undefined`, `NaN`的元素

- example

```js
_.compact([0, 1, false, 2, '', 3]);
// => [1, 2, 3]
```

### _.concat

- 生成一个新的数组，在尾部追加上额外的数组或者值

-example

```js
var array = [1];
var other = _.concat(array, 2, [3], [[4]]);

console.log(other);
// → [1, 2, 3, [4]]

console.log(array);
// → [1]
```

### _.difference(array, [values])

- 排除array数组中的values值, 生成一个新的数组, 不包含[values]数组中的值

- example

```js
_.difference([1, 2, 3], [4, 2]);
// => [1, 3]
```