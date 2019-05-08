# JavaScript Is Neat
Upon further inspection (after spending many hours writing JavaScript) I've discovered that the language is neat, mostly because of the way it is.

## Adding Booleans Together
Not sure who would ever do this but nonetheless it is valid.
```
const value = true + true - false;
console.log(value);
```
**Answer: 2**

When adding two booleans together true gets converted to 1, and false gets converted to 0 so: 1 + 1 - 2 = 2
