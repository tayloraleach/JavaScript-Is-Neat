# JavaScript Is Neat
Upon further inspection (after spending many hours writing JavaScript) I've discovered that the language is neat, mostly because of the way it is.

## Adding Booleans Together
Not sure who would ever do this but nonetheless it is valid.
```
const value = true + true - false;
console.log(value);
```
**Answer: 2**

When adding two booleans together true gets converted to 1, and false gets converted to 0 so: 1 + 1 - 0 = 2

## The Infamous Semicolon
```
const foobar = function() {
  return
  {
    name: 'jimmy'
  }
}
foobar();
```

I'm sure everyone has encountered this one but it's something that may get overlooked if you're getting quizzed on your skills and you're crunched for time.

This obviously returns `undefined` because the line with the return statement gets a semicolon added to it and the function it basically returns nothing.

## Are Strings Strings?
```
"hey I like to code" instanceof String
```
This one got me pretty good. Seems logical that a string is a string...
 but without explicitly calling the `new String()` constructor it is actually just an `object` and the above code returns false.
```
new String('js is fun') instanceof String
```
But this will obviously return true.
