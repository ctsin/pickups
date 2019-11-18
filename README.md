# console
## console.clear()
## console.assert(condition, "failure message")
```ts
var a = 10; 
console.assert(a === 10, "This will not be printed");
console.assert(a != 10, "this will be printed", `a = ${a}`);
// Assertion failed: this will be printed a = 10
```
## console.count()
```ts
function test() {
  console.count();
}

test(); // default : 1 
test(); // default : 2
test(); // default : 3

// Example 2 :We can also use label to it
function test(label) {
  console.count(label);
}
test("Times"); // Times: 1
test("Num"); // Num: 1test("Times"); // Times: 2
test("Num"); // Num: 2test("Times"); // Times: 3
test("Num"); // Num: 3
```

# console.countReset()
Resets the counter. This function takes an optional argument label.

```ts
console.count(); default: 1
console.count(); default: 2
console.count(); default: 3

console.countReset()
console.count(); default: 1
console.count("time"); time: 1
console.count("time"); time: 2
console.count("time"); time: 3
console.countReset()
console.count("time"); time: 1
```

## much more
`console.trace()`, `console.dir()`, `console.dirxml()` output HTML list, `console.table(obj)`, `console.group("days")` and `console.groupEnd("days")` group can be nested.
