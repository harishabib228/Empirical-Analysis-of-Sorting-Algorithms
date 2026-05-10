# Empirical-Analysis-of-Sorting-Algorithms

This project presents an empirical analysis of four fundamental sorting algorithms using Python. The assignment compares the performance, time complexity, and memory usage of different sorting techniques under multiple input conditions.

## Algorithms Implemented

The following sorting algorithms are implemented and analyzed:

1. Selection Sort
2. Bubble Sort
3. Quick Sort (Median-of-Three Pivot)
4. Merge Sort

## Objective

The objective of this project is to:

- Compare practical execution times of sorting algorithms
- Analyze the effect of input order on performance
- Verify theoretical Big-O complexities using empirical results
- Compare auxiliary space requirements
- Understand which algorithm performs best in different scenarios

## Technologies Used

- Language: Python
- Timing Function: `time.perf_counter()`
- IDE: VS Code / PyCharm / Any Python Environment

## Features

- Performance testing of sorting algorithms
- Comparison of sorted and reverse-sorted inputs
- Average execution time calculation
- Comparison counting and swap counting
- Auxiliary space analysis
- Big-O complexity verification

## Experimental Setup

Each algorithm was tested on:
- Sorted arrays
- Reverse-sorted arrays

Input sizes:
- n = 5
- n = 100

Each test case was executed 3 times and the average execution time was recorded in microseconds (µs).

## Performance Summary

| Algorithm      | Best Case  | Average Case | Worst Case | Auxiliary Space |
| -------------- | ---------- | ------------ | ---------- | --------------- |
| Selection Sort | O(n²)      | O(n²)        | O(n²)      | O(1)            |
| Bubble Sort    | O(n)       | O(n²)        | O(n²)      | O(1)            |
| Quick Sort     | O(n log n) | O(n log n)   | O(n²)      | O(log n)        |
| Merge Sort     | O(n log n) | O(n log n)   | O(n log n) | O(n)            |

## Key Observations

**Bubble Sort**
-Fastest for very small sorted arrays
- Early-exit optimization improves best-case performance
- Performs poorly on reverse-sorted large inputs
**Selection Sort**
- Performance is mostly unaffected by input order
- Makes fixed comparisons regardless of data arrangement
- Uses very little memory
**Quick Sort**
- Very efficient for large datasets
- Median-of-three pivot reduces worst-case behavior
- Requires recursive stack memory
**Merge Sort**
- Stable and consistently fast
- Guarantees O(n log n) performance
- Uses extra memory during merging

## Results

**Fastest for Small Data**
Bubble Sort performed best for very small sorted arrays because of its early-exit optimization.

**Fastest for Large Data**
Quick Sort and Merge Sort performed significantly faster than O(n²) algorithms for larger inputs.

**Memory Usage**
- Selection Sort and Bubble Sort used the least memory
- Merge Sort required the highest auxiliary space
- Quick Sort balanced performance and memory efficiency

## Conclusion

This project demonstrates that no single sorting algorithm is ideal for every situation. The performance of a sorting algorithm depends on:
- Input size
- Input order
- Memory constraints
- Required stability

For small datasets, simple algorithms like Bubble Sort and Selection Sort can perform well. For large datasets, Quick Sort and Merge Sort provide much better efficiency due to their O(n log n) complexity.

## Author
**Muhammad Haris Habib**
