# insertionSortRecursion
Insertion sort is another sorting algorithm that can be implemented recursively, although it's more naturally expressed iteratively. Nonetheless, implementing it recursively can be a good exercise in understanding recursive algorithms and sorting techniques. Here’s how you can implement Insertion Sort recursively in Java:


Explanation:
insertionSortRecursive Method:

This is the recursive function that sorts the array arr of size n using insertion sort.
Base case (if (n <= 1)) is reached when there is only one element left in the array, which is already sorted.
Recursive Call:

The function recursively sorts the first n-1 elements of the array (insertionSortRecursive(arr, n - 1)).
Insertion Logic:

After sorting the first n-1 elements recursively, the last element (arr[n-1]) is inserted into its correct position in the sorted array.
It compares the last element with the elements before it and shifts the greater elements one position to the right until it finds the correct position for the last element.
Main Method:

Initializes an array arr and prints it before and after sorting using the printArray method.
Calls insertionSortRecursive to start the recursive sorting process.
printArray Method:

Utility method to print the contents of an array.
Notes:
Recursive Insertion Sort has a time complexity of O(n^2), similar to its iterative counterpart, as each element is inserted into its correct position one by one.
The space complexity is O(n) due to the recursion stack space used by the function calls.
While recursive Insertion Sort is educational, iterative Insertion Sort is generally preferred for practical implementations due to its simpler implementation and better performance characteristics.
