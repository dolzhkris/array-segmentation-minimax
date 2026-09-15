# array-segmentation-minimax
Python program for generating array partitions into contiguous segments and finding the partition with the minimum maximum segment sum.

## About

The program divides an input array into k non-empty contiguous segments.

For each possible partition, it:

1. Calculates the sum of every segment.
2. Finds the maximum segment sum.
3. Displays the partition and its maximum sum.
4. Finds the partition where this maximum sum is minimal.

The program uses recursion and a generator to enumerate all possible partitions.

This project was developed as a university project during the third year of university.

## Key Functions

* gen_otr(a, k) - generates all possible partitions of array a into k non-empty contiguous segments.
* form_otr(start, parts_left, current) - recursive helper function used by gen_otr(). It builds the segments one by one and uses backtracking to generate different partition variants.
* print_var_and_find_min(a, k) - prints all generated partitions, calculates their maximum segment sums, and finds the minimum possible maximum.

## Key Variables

* a - input array;
* k - required number of contiguous segments;
* n - number of elements in the array;
* start - current position in the array from which a segment is formed;
* parts_left - number of segments remaining to be formed;
* current - list of segments already formed;
* variations - current generated partition;
* sums - sums of the segments in the current partition;
* max_sum - maximum segment sum for the current partition;
* min_max_sum - minimum maximum segment sum found so far;
* best_var - best partition found by the program;
* i - position used to determine the end of the next segment.

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/dolzhkris/array-segmentation-minimax.git
```

2. Run the program:

```bash
python main.py
```

Enter n and k in one line. Then enter the array.

Computer Engineering Graduate
Junior Python Developer
