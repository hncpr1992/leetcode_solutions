# leetcode 
  -- # 88
  
## Tips
1. Care about the special cases<br>
2. Think in diverse directions<br>
3. <br>


## Easy
### Array
1.Two Sum -> Use hash table to avoid going through the list <br>
448.Find All Numbers Disappeared in an Array -> 1.Build a buffer to count the numbers | 2.Use the array as a buffer with sign <br>
118.Pascal's Triangle -> understand structure and do it<br>
167	Two Sum II - Input array is sorted: Use the condition of sorted array, use the two pointers at front and rear<br>
35.Search Insert Position -> linear search / binary search (left and right has 1 gap) <br>
66.Plus One -> understand the process of addition<br>
122.Best Time to Buy and Sell Stock II -> dynamic programming -> <br>
27.Remove Element -> Two pointers, front and rear, swap<br>
268.Missing Number -> the sum of numbers　[0,1,2,...,n] is a constant, so the missing one can be calculated<br>
169.Majority Element -> Hashtable | Boyer–Moore majority vote algorithm<br>
283.Move Zeroes -> 27.Remove Element<br>
243.Shortest Word Distance -> Move forward and record the words position to calculate distance<br>
219.Contains Duplicate II -> 243.Shortest Word Distance with a buffer recording multiple elements' index<br>
217.Contains Duplicate -> 219.Contains Duplicate II Hash table or buffer<br>
119.Pascal's Triangle II -> Next one add to the prior one and get the number in next row<br>
26.Remove Duplicates from Sorted Array -> move and swap, two pointers | 27.Remove Element, 283.Move Zeroes<br>
189.Rotate Array<br>
186.Reverse Words in a String II<br>
414.Third Maximum Number -> A slide window that capture the first second and third<br>

### Dynamic Programming
121.Best Time to Buy and Sell Stock -> get today's maxprofit based on yesterday's<br>
122.Best Time to Buy and Sell Stock II<br>
53.Maximum Subarray<br>
198.House Robber -> build a recurrence relation
70.Climbing Stairs -> build a recurrence relation <br>

256.Paint House -> Use previous steps' costs as base and get new min costs<br>
276.Paint Fence -> Same or not Same situations<br>
303.Range Sum Query - Immutable -> Cumsum in a list to get sum of a slice<br>

### Linked List
206.Reverse Linked List -> keep the code in mind<br>
141.Linked List Cycle -> fast and slow pointers<br>
83.Remove Duplicates from Sorted List -> Use the sorted condition <br>
203.Remove Linked List Elements -> take care of the situation that head.val == val<br>
237.Delete Node in a Linked List -> copy next and remove next<br>
234.Palindrome Linked List -> two poiinters with half reversing<br>
160.Intersection of Two Linked Lists -> scan two lists in a loop until find first common node<br>
21.Merge Two Sorted Lists -> merge one node by another O(m+n)<br>

### Hash table
349.Intersection of Two Arrays -> build a hash table and check existence<br>
350.Intersection of Two Arrays II -> hash table but keep the amount of numbers<br>
438.Find All Anagrams in a String -> slide window and form hash table each step<br>
205.Isomorphic Strings　-> build hash table along the way<br>
359.Logger Rate Limiter -> build hash table along the way<br>
204.Count Primes -> Sieve of Eratosthenes<br>


409.Longest Palindrome -> do not iterate to find, learn how to calculate the result, get the pattern<br>
447.Number of Boomerangs -> see the pattern and calculate, build a hash table to store the distance<br>
389.Find the Difference -> trade space for time<br>
246.Strobogrammatic Number -> build a rule and check<br>
242.Valid Anagram -> 389.Find the Difference<br>
136.Single Number -> hash | bit manipulation<br>
290.Word Pattern -> 205.Isomorphic Strings<br>
170.Two Sum III - Data structure design -> Two sum<br>
266.Palindrome Permutation -> 409.Longest Palindrome<br>
202.Happy Number -> build along the way | two pointers (cycle)<br>

### Two pointers
125.Valid Palindrome -> skip punctuations and other<br>
345.Reverse Vowels of a String -> reverse a list with hash table as vowels<br>
344.Reverse String -> just reverse with two pointers<br>

### Stack
155.Min Stack -> remember to use a minStack array to keep the minimum for each push<br>
20.Valid Parentheses -> use a stack to match the input parenthesis<br>
***496.Next Greater Element I -> Use a stack to keep the decreasing sequence***<br>
232.Implement Queue using Stacks -><br>
225. Implement Stack using Queues -><br>

### String
344.Reverse String -> two pointers<br>
13.Roman to Integer -> if left number is smaller than the right number, subtract the left one from the total<br>
293.Flip Game -> slide window to flip<br>
520.Detect Capital -> follow the rules and compare three situations<br>

### Tree
226.Invert Binary Tree -> recurse to flip left and right <br>
270.Closest Binary Search Tree Value -> make your code simple<br>
***235.Lowest Common Ancestor of a Binary Search Tree -> Compare the two nodes' values with root, if at two side, return root, else go left or right***<br>
112.Path Sum -> take the sum at last recursion as argument in the next recursion and manipulate<br>
257.Binary Tree Paths -> dfs<br>
111.Minimum Depth of Binary Tree -> dfs -> 257<br>
100.Same Tree -> compare left , right structure and the root value in recursion<br>
101.Symmetric Tree -> Same as the 100 Same Tree, but compare the left with the right<br>
104.Maximum Depth of Binary Tree -> Same as the 111.Minimum Depth of Binary Tree, but use max<br>
404.Sum of Left Leaves -> memorize the code as a sample<br>
110.Balanced Binary Tree -> memorize the code as a sample | use some value as signals<br>
108. Convert Sorted Array to Binary Search Tree -> memorize the code <br>

### Math
258.Add Digits -> use // and %<br>
171.Excel Sheet Column Number -> calculate like a number<br>
172.Factorial Trailing Zeroes -> Find how many 5 we have n/5 + n/25 + n/125 + n/625 + n/3125+...<br>
202.Happy Number -> when there is a cycle, use two pointers<br>
7.Reverse Integer -> get number by //10 and reverse, set condition for overflow<br>
9.Palindrome Number -> Use % 10 and // 10 in flexible way<br>
453.Minimum Moves to Equal Array Elements -> transform the issue from add to subtract<br>
69.Sqrt(x) -> binary search<br>
204.Count Primes -> memorize the mothod <br>
168.Excel Sheet Column Title -> reduce 1-10 to 0-9<br>
441.Arranging Coins -> you can add number, but you can also subtract number<br>
231. Power of Two -> same as 441.Arranging Coins<br>

### DFS
339.Nested List Weight Sum -> DFS with recursion on nested list<br>

### BFS
107.Binary Tree Level Order Traversal II -> typical BFS algo<br>



## Medium
Ordered by frequency<br>
-- # 15

2.Add Two Numbers -> Go through two list until empty | add == 1 or 0 <br>
6.ZigZag Conversion -> make sure the period of the string character collection<br>
3.Longest Substring Without Repeating Characters -> two pointers and dynamic hash table<br>
388.Longest Absolute File Path -> hash table + loop <br>
12.Integer to Roman -> follow the rule, go from large number to small number<br>
***5.Longest Palindromic Substring ->***

540.Single Element in a Sorted Array -> logn indicate binary search, use odd or even amount as the criteria<br>
238.Product of Array Except Self -> two pointers from left to right with an output array<br>
328.Odd Even Linked List -> two pointers slow and fast, do not make mistake at exchange link list nodes<br>
***338. Counting Bits***<br>
***148. Sort List***<br>

***139.Word Break***<br>
***137. Single Number II -> bit manipulation | hash table***<br>
17.Letter Combinations of a Phone Number -> iterate one digit by another<br>
***50. Pow(x, n)***<br>
***200. Number of Islands***<br>

319.Bulb Switcher -> brain teaser (the factorial come as pairs except for n^2) so just get the square root<br>
153. Find Minimum in Rotated Sorted Array -> binary search<br>
49. Group Anagrams -> sort the string characters and use hash table to store them<br>
22. Generate Parentheses -> backtracking<br>
150. Evaluate Reverse Polish Notation -> stack<br>





  



