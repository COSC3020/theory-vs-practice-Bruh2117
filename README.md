[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12049056&assignment_repo_type=AssignmentRepo)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.
  - The constant factor $c$ could be ignored 
  - $n_{0}$ could be ignored  
  - Hardware constraints could be ignored 

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  - Since the asymptotic complexity of a binary search tree is $O(log_{2}(n))$ for $n$ elements, we can solve for constant $c$ that's multiplied with the function $f(n)$ from the asymptotic notation. To do this, from the first search specified, we can divide 5 by $log_{2}(1000)$ to get get our constant factor $c$, which is approximately $0.502$. With that, we can now calculate the runtime for the case of searching for the same element in a 10,000 element tree, which will $c*log_{2}(n) = 0.502*log_{2}(10,000) =$ 6.67 seconds. 

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.
  - The first reason could be hardware constraints, such as limited memory
  - The second could be things running in the background while doing the search on the computer, slowing the CPU down immensely
  - The third could be that the tree is imbalanced, causing the search to go slower than expected

Add your answers to this markdown file.
