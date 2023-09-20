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


Using asymptotic complexity, if a binary search tree with 1,000 elements takes 5 seconds, a binary search tree with 10,000 elements would take roughly 3 times longer. The time complexity of a binary search tree is O(h), where h is the height. The asymptotic complexity of a tree is O(logN). If you 10,000 elements and divide it by the elements for the case that took 5 second, 10,000/1,000 you get 10. If you take log base 2 of 10, you roughly get three, which is the ratio of the two compared. So the time of a list with 1,000 elements takes 5 seconds, and the time that a list of 10,000 elements would tak is, Log base 2 (10)= 3 * 5 seconds = 15 seconds. 

If the tree is unbalanced, this can change the time complexity to worst case scenario, O(N). This would take much longer to search the tree. It could also be a low order term that does not grow effectively and effects the results. If the implementation of the search algorithm is not an efficient one, it might not work as well with a larger number of elements. This would defintely lead to longer search times. 

(I used ChatGPT to check what constant factors did to asymptotic analysis)
(I had James Osborn look at my questions, and I he helped me fix the first and third part.) 
