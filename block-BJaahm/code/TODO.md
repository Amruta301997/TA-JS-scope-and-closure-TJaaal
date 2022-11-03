1. Construct a function intersection that compares input arrays and returns a new array with elements found in all of the inputs. You can only use reduce method to do this.

```js
function intersection(arrays) {
   array = [];
  for (var i = 0; i < arguments.length; i++)
    array.push(arguments[i]);

  var result = [];

  for(var i = 0; i < array.length - 1; i++) {
    for(var j = 0; j < array[i].length; j++) {
      if (array[i+1].includes(array[i][j]))
        result.push(array[i][j]);
    }
  }

  return result;
}

// Test
console.log(
  intersection(
    [5, 10, 15, 20],
    [15, 88, 1, 5, 7],
    [1, 10, 15, 5, 20]
  )
); // should log: [5, 15]
```

2. Construct a function `union` that compares input arrays and returns a new array that contains all elements. If there are duplicate elements, only add it once to the new array. Preserve the order of the elements starting from the first element of the first input array. You can only use reduce method to do this.

```js
function union(arrays) {
   return arrays.reduce((acc, array) => {
    const newItem = array.filter((item) => !acc.includes(item));
    return acc.concat(newItem);
  });
}

// Test
console.log(
  union([5, 10, 15], [15, 88, 1, 5, 7], [100, 15, 10, 1, 5])
);
// should log: [5, 10, 15, 88, 1, 7, 100]
```
