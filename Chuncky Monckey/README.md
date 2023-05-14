

# chunkArrayInGroups

The `chunkArrayInGroups` function is a utility function that splits an array into smaller subarrays of a specified size.

## Usage

```javascript
const arr = [1, 2, 3, 4, 5, 6, 7, 8];
const size = 3;

const result = chunkArrayInGroups(arr, size);
console.log(result);
// Output: [[1, 2, 3], [4, 5, 6], [7, 8]]
```

## Parameters

- `arr` (Array): The array to be chunked.
- `size` (number): The size of each subarray.

## Return Value

(Array): An array containing the resulting subarrays.

## Example

```javascript
const arr = [1, 2, 3, 4, 5, 6, 7, 8];
const size = 3;

const result = chunkArrayInGroups(arr, size);
console.log(result);
// Output: [[1, 2, 3], [4, 5, 6], [7, 8]]
```

## Implementation

The `chunkArrayInGroups` function iterates over the input array and collects elements into a temporary array until the size of the temporary array reaches the specified `size`. Once the temporary array reaches the desired size, it is added to the `result` array, and the temporary array is reset to an empty array. Any remaining elements that did not complete a full subarray are added to the `result` array after the loop. Finally, the `result` array is returned.

Please note that the `chunkArrayInGroups` function assumes that the input `arr` is an array and the `size` is a positive integer.

Feel free to modify and use this function according to your requirements!

## License

This code is released under the [MIT License](https://opensource.org/licenses/MIT).
