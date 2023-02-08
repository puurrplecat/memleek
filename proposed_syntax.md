# Syntax and Grammar

Basic types: 
u8, u16, u32, u64, u128?, i8, i16, i32, i64, i128?, char, str, bool, [x] (array), (x) (tuple), 

<br>
Variable assignment and type annotation

``` x: u32 = 10; ```

```x``` is variable name, ```:``` is separator, the spacing after is optional, ```=``` is assignment (type inference? type checking?)
(Should we make colon optional?)

<br>
Conditionals

``` 
if x == 2 {
  ...
} else if x == 3 {
  ...
} else {
  ...
}
```

I prefer the no bracket around condition.

<br>
For loop

```
 for i in [0,100] {
    print(i)
 }
```
For basic numeric range, we use mathematic's interval notation. (For now, to loop through array, we must loop through a range of numbers that index the array

<br>
While loop

```
while x < 0 {
  x += 1
}
```

<br>
Functions

```
x( a: u32, b: u32, c: u32) : u32 {
  ...
}
```

Debate for ```return``` keyword

<br>
Structs

```
class X<T> A B C {
  a: u32
  b: T
  methods {
    p(...) {...}
  }
}
```
This class is generic over type T and must have the classes A, B, C built for X. For an example of A, see below

<br>
Composition over inheritance as a fundamental design princple.

```
superclass A {

  m (self) : u32 {
    self.a + 1
  }
}
```
the superclass (needs better name) define methods that are shared behaviour (idk how to type check this)

<br>
Enums

```
enum Human {
  Male,
  Female
}
```
Comma is optional
