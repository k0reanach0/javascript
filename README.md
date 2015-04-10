# javascript
Javascript - Helpful Stuff

#### EVEN ODD EVEN ODD
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

#### SWAP CHARACTERS
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
######

#### ITERATE ARRAY - BACKWARDS
```javascript
for (var i = array.length - 1; i >= 0; i--) {
  // CODE
}
```
