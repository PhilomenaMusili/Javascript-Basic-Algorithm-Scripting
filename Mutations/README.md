# Mutation Function

This repository contains a JavaScript function called `mutation` that checks if all the characters in one string are present in another string, regardless of case sensitivity.

## Usage

To use the `mutation` function, follow these steps:

1. Include the `mutation` function in your JavaScript code.

```javascript
function mutation(arr) {
  return arr[1]
    .toLowerCase()
    .split("")
    .every(function(letter) {
      return arr[0].toLowerCase().indexOf(letter) !== -1;
    });
}

Call the mutation function with an array of two strings as an argument. The first string represents the target string, and the second string represents the test string.
  
const result = mutation(["hello", "oleh"]);
console.log(result); // Output: true

In the above example, the mutation function will return true because all the characters in the test string "oleh" are present in the target string "hello".

## Function Explanation

The mutation function performs the following steps to determine if all characters in the test string are present in the target string:

Convert the test string to lowercase using .toLowerCase() to ensure case insensitivity.
  
Split the lowercase test string into an array of individual characters using .split("").
  
Iterate over each character in the test string using .every(function(letter) { ... }).
  
Within the iteration, check if the current character exists in the target string by using .toLowerCase().indexOf(letter) !== -1.
  
  This returns true if the character is found and false otherwise.
    
The .every() method returns true if all characters in the test string are found in the target string, and false otherwise.

  ## License
This project is licensed under the MIT License.






