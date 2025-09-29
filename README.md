# EXPERIMENT NO – 20

* Aim: To study and implement searching techniques in C++ for finding elements in arrays.

* Tools Used: IDE, C++ compiler, arrays, functions, linear search, binary search.

* Theory:

In C++, searching is the process of locating a specific element within a data structure such as an array. It is an essential operation in programming to retrieve data efficiently.

-Searching helps in finding whether an element exists and its position in a collection.

-Different algorithms are used depending on whether the data is sorted or unsorted.

🔹 *Key Features of Searching:*

* Enables retrieval of data from arrays or other data structures.

* Supports both sorted and unsorted collections (depending on the method).

* Returns the index of the found element or indicates absence.

* Essential for applications requiring data lookup, filtering, or validation.

🔹 *Types of Searching in C++:*

i> Linear (Sequential) Search – Checks each element in order until the target is found.

*Syntax:*

    int linearSearch(int arr[], int size, int target) {
    for (int i = 0; i < size; i++) {
        if (arr[i] == target)
            return i;
    }
    return -1;
    }


ii> Binary Search – Efficient search on sorted arrays by repeatedly dividing the search interval in half.

*Syntax:*

    int binarySearch(int arr[], int size, int target) {
    int start = 0, end = size - 1;
    while (start <= end) {
        int mid = start + (end - start) / 2;
        if (arr[mid] == target)
            return mid;
        else if (arr[mid] < target)
            start = mid + 1;
        else
            end = mid - 1;
    }
    return -1;
    }


🔹 *Advantages of Searching:*

* Allows fast and efficient retrieval of elements.

* Essential for database queries, sorting, and algorithmic operations.

* Forms the foundation for more advanced search algorithms.

* Helps in validating and filtering data.

# Conclusion:

Searching implementation in C++ demonstrates how elements can be located in arrays effectively. Linear search is simple and works on any array, while binary search is faster for sorted arrays. Understanding these methods is fundamental for data handling and algorithm design.
