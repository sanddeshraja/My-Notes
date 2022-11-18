 - Rough Soln./ FlowChart is called pseudocode
- FlowChart -> High Level Language(Java) -> machine code (0's and 1's)
- Diagramatic repn. of approach to solve the problem

## FlowChart

![[DSA 2022-10-19 21.53.36.excalidraw]]

![[DSA 2022-10-19 21.56.17.excalidraw]]

![[DSA 2022-10-19 21.57.08.excalidraw]]

![[DSA 2022-10-19 21.58.03.excalidraw]]

![[DSA 2022-10-19 21.59.28.excalidraw]]

## PseudoCode

Way of representing logic to solve the problem
No specidic way to represent


## Types Of Languages

1.  Procedural
2.  Functional 
3.  Object Oriented

or

1. Static Language
2. Dynamic Language



## Linear Data Structure

Time complexity
 
Best : o(1)  Worst : o(N)


## Binary Search

time complexity

Best: O(1) Worst: O(log   N)
                                     2
                                     
N/2^k=1
N=2^K
logN=Log2^K
k=log N
         2

<code>
 while(start &lt; =end)
 {
   int mid = start + (end-start)/2;
   if target &lt arr[mid]
   {
     end=arr[mid]-1
   }
   else
   {
   start=arr[mid]+1
   }
 }
</code>
 
