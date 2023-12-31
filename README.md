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

Three reasons what asymptotic analysis may be misleading with respect to actual performance in practice are hardware differences, constant factors, and run time variability. 

1. When an algorithm is ran on two seperate computers, if one computer has better hardware it will run faster. This can be misleading if the two computers are comparing times. This can be the case for two equal computers as well, just with slightly different parts, there is factors like the memory and CPU that could change results. 

2. An algorithm can ignore constant factors when using asymptotic analysis. Larger constant factors can make the algorithm slower for practical input sizes.
  
3. Two algorithms with the same asymptotic complexity may have different actual run times due to variations in their internal operations, data strucutres used, and efficiency of implementation.  


The asymptotic time complexity of a binary serach tree is O(log n). The best way to find the run time will be to take the ratio of 1,000 elements and 10,000 elements. To do this we can do the following calculation, log(1,000) = 9.97, log(10,000) = 13.29. Do the calculation ((13.29/9.97) * 5) and we get that the run time will be apporxiamtly 6.66 seconds. 

1. It could be the case that the first time this algorithm was ran the element was the root of the tree, which would be best case scenario. Meaning it would not be seen as slow if it was only ran one time and that one time was best case, that would make it shocking to find the increased runtime. From the drastic change it could be the worst case or even average case for the second run with more elements. 
 
2. If the implementation of the search algorithm is not an efficient one, it might not work as well with a larger number of elements. This would defintely lead to longer search times. There could be various reasons why it would not work with a larger input size such as innefficient operations, ineffective search strategies, and inadequate indexing or sorting. An example of inefficent opertions could be nested loops with higher iterations or redundant calculations. An example of the use of ineffective search strategies would be if the search had to look at a large portion of the elements before finding the solution. An example of inadequate indexing or sorting would be if the algorithm relies on linear search or even lacks efficent indexing or sorting mechanisms. 

3. Another reason might be the hardware of the computer. If the larger tree exceeds the available RAM, it may result in more frequent disk I/O operations, causing a significant slowdown in the search process. Additionally, if the search algorithm or data structures used have higher memory requirements, the larger dataset could lead to increased paging, swapping, or other memory-related issues, impacting performance.

(I used ChatGPT to check what constant factors did to asymptotic analysis)

(I had James Osborn look at my questions, and I he helped me fix the first and third part.) 

(Calculation errors in part 2)
