# Bonus: Quicksort

**Fork and then clone me!**

![quicksort animation](./quick_sort_partition_animation.gif)

Quicksort is an efficient divide and conquer algorithm for sorting data. It can sort in place, i.e. it does not require us to push data to a new data structure, and it's typically implemented as a recursive algorithm. Note that there are a number of ways to implement a quicksort.

## How Does Quicksort Work?

The quicksort algorithm requires us to choose a pivot element in the array. The pivot can be at any point, such as the start, middle, or end. Next, we sort all of the elements that are less than the pivot to the left of the pivot, and all of the elements that are greater than the pivot to the right. Once this is done, the pivot is at the correct location. We then repeat this process on the left and right sides until the whole list is sorted. 

In the diagram below, notice how the number 4, which is the pivot, is sorted to the correct location before the recursive call is made (branching denotes the recursive calls). First, we check if 1 is more than 4. It isn't so we move to the next value: 7. 7 is more than 4, so it is swapped with the element before 4 (which is 5), and 4 is then swapped with 7. This continues until every element before the pivot has been evaulated.

![diagram of quicksort in action](./quicksort_diagram.png)

## Performance

In the worst case, quicksort runs in quadratic time: O(n^2). This will happen when we choose the rightmost element as the pivot for an already sorted list. The average run time, however, is logarithmic: O(n log n). 

We can improve the performance of our quicksort algorithm by choosing the middle element as the pivot instead. We can potentially gain further improvements by sampling three or more elements and choosing the median as the pivot. However, choosing too many elements for sampling will likely degrade performance, so it really is a balancing act.

## Implement Quicksort

Use the language of your choosing. We've included starter files for some languages where you can pseudocode, explain your solution and code.

## Before you start coding:

1. Rewrite the problem in your own words
2. Validate that you understand the problem
3. Write your own test cases
4. Pseudocode
5. Code!

**_And remember, don't run our tests until you've passed your own!_**

## How to run your own tests

### Ruby

1. `cd` into the ruby folder
2. `ruby <filename>.rb`

### JavaScript

1. `cd` into the javascript folder
2. `node <filename>.js`

## How to run our tests

### Ruby

1. `cd` into the ruby folder
2. `bundle install`
3. `rspec`

### JavaScript

1. `cd` into the javascript folder
2. `npm i`
3. `npm test`
