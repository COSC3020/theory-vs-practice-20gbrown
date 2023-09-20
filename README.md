[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11862619&assignment_repo_type=AssignmentRepo)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

Three reasons what asymptotic analysis may be misleading with respect to actual performance in practice are hardware, constant factors, and run times. When an algorithm is ran on two seperate computers, if one computer has better hardware it will run faster. This can be misleading if the two computers are comparing times. This can be the case for two equal computers as well, just with slightly different parts, there is factors like the memory and CPU that could change results. An algorithm can ignore constant factors when using asymptotic analysis. Larger constant factors can make the algorithm slower for practical input sizes. Something else that can be misleading about asymptotic analysis is that two algorithms may have the same asymptotic complexity but have different run times. 


The asymptotic time complexity of a binary serach tree is O(log n). The best way to find the run time will be to take the ratio of 1,000 elements and 10,000 elements. To do this we can do the following calculation, log2(10,000) = 13.29. We can use the value of 5 seconds for 1,000 elements to figure out the time for 10,000 elements. Do the calculation (13.29 * 5) and we get that the run time will be apporxiamtly 66.54 seconds. (I'm not sure if I am failing to understand this, or if I need to do log2(10,000)/log2(1000) and take that number times 5).

If the tree is unbalanced, this can change the time complexity to worst case scenario, O(N). This would take much longer to search the tree. This could also be caused by memory and cache behavior, caches misses and memory access patterns would slow search times down.  If the implementation of the search algorithm is not an efficient one, it might not work as well with a larger number of elements. This would defintely lead to longer search times. 

(I used ChatGPT to check what constant factors did to asymptotic analysis)
(I had James Osborn look at my questions, and I he helped me fix the first and third part.) 
(Calculation errors in part 2)
