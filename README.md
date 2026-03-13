# Simple-Insertion-sort-program-
Data structure practical program 
# Insertion Sort in Python

def insertion_sort(arr):
    n = len(arr)
    for i in range(1, n):
        key = arr[i]
        j = i - 1
        # Move elements greater than key to one position ahead
        while j >= 0 and arr[j] > key:
            arr[j + 1] = arr[j]
            j -= 1
        arr[j + 1] = key

# Example usage
arr = [12, 11, 13, 5, 6]
print("Original array:", arr)

insertion_sort(arr)
print("Sorted array:", arr)

output:
Original array: [12, 11, 13, 5, 6]
Sorted array: [5, 6, 11, 12, 13]
