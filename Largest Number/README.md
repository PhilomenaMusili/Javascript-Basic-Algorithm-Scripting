# Largest Number in Sub-Arrays

This repository contains a JavaScript function named `largestOfFour` that finds the largest number in each sub-array within a given array `arr`. It returns an array containing the largest numbers.

## Usage

To use the `largestOfFour` function, follow these steps:

1. Copy the code from the `largestOfFour.js` file.
2. Paste the code into your JavaScript project.

```javascript
function largestOfFour(arr) {
  const results = [];
  for (let i = 0; i < arr.length; i++) {
    let largestNumber = arr[i][0];
    for (let j = 1; j < arr[i].length; j++) {
      if (arr[i][j] > largestNumber) {
        largestNumber = arr[i][j];
      }
    }
    results[i] = largestNumber;
  }

  return results;
}
```

3. Call the `largestOfFour` function with an array of arrays as an argument. Each sub-array should represent a set of numbers.
4. The function will find the largest number in each sub-array and return an array containing the largest numbers.

Example:
```javascript
const result = largestOfFour([[4, 5, 1, 3], [13, 27, 18, 26], [32, 35, 37, 39], [1000, 1001, 857, 1]]);
console.log(result);
```

Output:
```
[5, 27, 39, 1001]
```

This indicates that the largest numbers in the provided sub-arrays are `[5, 27, 39, 1001]`.

Feel free to use the `largestOfFour` function in your JavaScript projects when you need to find the largest numbers in sub-arrays.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code for your own purposes.
