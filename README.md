# javascript
Javascript - Helpful Stuff

#### Even Odd Even Odd
```javascript
for (var y = 0; y < size; y++) {
  for (var x = 0; x < size; x++) {
    if ((x + y) % 2 == 0)
      board += " ";
    else
      board += "#";
  }
  board += "\n";
}
```

#### Swap Characters
```javascript
function reverseArrayInPlace(array) {
  for (var i = 0; i < Math.floor(array.length / 2); i++) {
    var old = array[i];
    array[i] = array[array.length - 1 - i];
    array[array.length - 1 - i] = old;
  }
  return array;
}
```

#### Iterate Array - Backwards
```javascript
for (var i = array.length - 1; i >= 0; i--) {
  // CODE
}
```

#### List Data Structure
```javascript
function arrayToList(array) {
  for (var i = array.length - 1; i >= 0; i--) {
    var list = {
      value: array[i],
      rest: list
    };
  }
  return list;
}

console.log(arrayToList([10, 20]));
```

#### Reading List Data Structure
```javascript
function listToArray(list) {
  var array = [];
  /*
   * node = list is only called once. Establishing the variable.
   * node; Condition While node is true;
   * node = node.rest; Incrementer - move to nested object.
   */
  for (var node = list; node; node = node.rest) {
    array.push(node.value);
  }
  return array;
}

console.log(listToArray(arrayToList([10, 20, 30])));
```
