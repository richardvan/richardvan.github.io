---
layout: page
title: Computer Science 
description: to learn
---
> Edsger Djikstra: "Computer science is no more about computers than astronomy is about telescopes."

---

### Big-O Notation
---

* **O(1):** *"constant time"*

      retrieving an element from an array. We know exactly where it is in memory, so we just go get it. It doesn't matter if the collection has 10 items or 10000; it's still at index (say) 3, so we just jump to location 3 in memory.
* **O(n):** *"linear time"*

      retrieving an element from a linked list. Here, A = 0.5, because on average you''ll have to go through 1/2 of the linked list before you find the element you're looking for. Even tradeoff for input versus time it takes, three times the input size will take roughly three times as long
* **O(n^2):** *"quadratic"*

      various "dumb" sorting algorithms. Because generally their strategy involves, for each element (n), you look at all the other elements (so times another n, giving n2), then position yourself in the right place.
* **O(n log(n)):** *"better than quadratic"*

      various "smart" sorting algorithms. It turns out that you only need to look at, say, 10 elements in a 1010-element collection to intelligently sort yourself relative to everyone else in the collection. Because everyone else is also going to look at 10 elements, and the emergent behavior is orchestrated just right so that this is enough to produce a sorted list.
* **O(n!):** *"brute force"*

      an algorithm that "tries everything," since there are (proportional to) n! possible combinations of n elements that might solve a given problem. So it just loops through all such combinations, tries them, then stops whenever it succeeds.

<img src="../../assets/pics/time-complexity.png"/>

```
Big-O       |  computations for 10 things |  for 100 things  | example
------------------------------------------------------------------------------------
O(1)        |   1                         |     1            | hash look-up
O(log(n))   |   3                         |     7            | 
O(n)        |  10                         |   100            | 
O(n log(n)) |  30                         |   700            | merge sort, heap sort, quick sort
O(n^2)      | 100                         | 10000            | bubble sort, insertion sort

```

---

### Sorting Algorithms in Action
---

  <embed src="../../assets/gifs/sortingAlgorithms.mp4" width="460" height="232" loop="true"/>
	