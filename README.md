Download Link: https://assignmentchef.com/product/solved-comp-352-data-structure-and-algorithms-assignment-2
<br>
<strong> </strong>




Computer Science and Software Engineering

Written Questions




<h1>Question 1</h1>

<strong> </strong>

Consider the algorithm <em>DoSomething</em> below:




<strong>Algorithm</strong> <em>DoSomething</em> (A, n)

<strong>  Input: </strong>Array A of integer containing n elements

<strong>Output:  </strong>Array S of integer containing n elements

<ol>

 <li><strong><em>for</em></strong><em> i=0 to n-1 <strong>do</strong> </em></li>

 <li><em>Var[i]=0 </em></li>

 <li><strong><em>end for </em></strong></li>

 <li><strong><em>for</em></strong><em> i=0 to n-2 <strong>do</strong> </em></li>

 <li><strong><em>for</em></strong><em> j=i+1 to n-1 <strong>do</strong> </em></li>

 <li><strong><em>if</em></strong><em> A[i]</em><em>A[j] <strong>then</strong> </em></li>

 <li><em>Var[j]= Var[j]+1 </em></li>

 <li><strong><em>else </em></strong></li>

 <li><em>Var[i]= Var[i]+1 </em></li>

 <li><strong><em>end if </em></strong></li>

 <li><strong><em>end for </em></strong></li>

 <li><strong><em>end for </em></strong></li>

 <li><strong><em>for</em></strong><em> i=0 to n-1 <strong>do</strong> </em></li>

 <li><em>S[Var[i]]= A[i] </em></li>

 <li><strong><em>end for </em></strong></li>

 <li><strong><em>Return</em></strong><em> S </em></li>

</ol>




<ol>

 <li>What is the big-O (<em>O(n)</em>) and big-Omega (<em>Ω(n)</em>) time complexity for algorithm <em>DoSomething</em> in terms of <em>n</em>? Show all necessary steps.</li>

 <li>Trace (hand-run) <em>DoSomething</em> for an array A = (60,35,81,98,14,47). What is the resulting A?</li>

 <li>What does <em>DoSomething</em> do? Explain that clearly and briefly given any arbitrary array A of n integers?</li>

 <li>Can the runtime of <em>DoSomething</em> be improved easily? Explain how (i.e., re-write another solution(s) that does exactly what <em>DoSomething </em>is doing more efficiently)?</li>

 <li>Can the space complexity of <em>DoSomething</em> be improved? Explain how?</li>

</ol>







<h1>Question 2</h1>







A company is involved in shipping large number of containers at a dock. Containers are classified into three categories:

<u>Category 1:</u> containers need to be accessed by their indices:  <em>lookup</em>, <em>set</em>, <em>add</em> and <em>remove</em> from Category 1. <u>Category 2:</u> containers need to be <em>add</em>ed and <em>removed</em> before or after certain position including the first and last position of the Category 2.

<u>Category 3:</u> containers need to be <em>added </em>and<em> removed</em> in a sorted alphabetical order of their destination and any new added container need to follow that order of the Category 3.




From the three linear ADTs: List, Positional and Sequence covered in class. discuss which ADT to choose and its underlying implementation for the above containers’ categories.










<h1>Question 3</h1>




<ol>

 <li>Draw a <u>single</u> binary tree that gave the following traversals:</li>

</ol>




Inorder:       C   O   P   Y   R   I   G   H   T   A   B   L   E

Postorder:   C   P   O   R   G   I   T   H   B   A   E   L   Y




<ol>

 <li>Assume that the binary tree from the above- part (a)- is stored in an array-list as a complete binary tree as discussed in class. Specify the contents of such an array-list for this tree.</li>

</ol>

<h1>Question 4</h1>




<ol>

 <li>Draw the min-heap that results from the bottom-up construction algorithm on the following list of values: 10,12,13,15,4,16,8,9,2,20,7,14,6,23,19</li>

</ol>




Starting from the bottom layer, use the values from left to right as specified above. Show immediate steps and the final tree representing the min-heap.




<ol>

 <li>Perform the operation removeMin two times on the heap you created in part (a) and show the resulting min-heap after each step and the final tree representing the min-heap.</li>

</ol>







<h1>Question 5</h1>




<ol>

 <li>Given a tree T, where <em>n </em>is the number of nodes of <em>T</em>.</li>

</ol>

Give an algorithm for computing the depths of all the nodes of a tree T. What is the complexity of your algorithm in terms of Big-O?

<ol>

 <li>We say that a node in a binary search tree is full if it has both a left and a right child.</li>

</ol>

Write an algorithm called <em>Count-Full-Nodes(t)</em> that takes a binary search tree rooted at node t, and returns the number of full nodes in the tree. What is the complexity of your solution?

<strong> </strong>

<strong> </strong>




<h1>Programming Questions</h1>

<strong> </strong>

In these programming questions you will evaluate two implementations of <em>List </em>interface in terms of their performance for different operations.




<em>List</em><a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a> interface is an ordered collection (also known as a <em>sequence</em>). The user of this interface has precise control over where in the list each element is inserted. The user can access elements by their integer index (position in the list), and search for elements in the list.

The List interface provides four methods for index <strong>access </strong>to list elements, two methods to <strong>search </strong>for a specific object, and two methods to efficiently <strong>insert </strong>and <strong>remove </strong>multiple elements at an arbitrary location in the list. Note that the speed of these operations may depend on the implementation (e.g., Array or LinkedList).




You are required to write two implementations of <em>List</em> interface, one that uses <u>array</u>, and one that uses <u>doublylinked list</u>. Then, you will have to test the performance of several operations when using your implementations.




Question 1:

<strong> </strong>

Implement the following methods in the two implementations (called <em>MyArrayList</em> and MyLinkedList) of List interface:




Boolean   add(E e)           // Appends the specified element to the end of this list void add(int index,E element) // Inserts the specified element at the specified position in this list void <sub> clear()</sub>                                     // Removes all of the elements from this list

E  remove(int index)         // Removes the element at the specified position in this list

Boolean remove(Object o)     // Removes the first occurrence of the specified element from this list

String  toString()               // Returns a string representation of this list int size()                  // Returns the number of elements in this list

<strong> </strong>

Define your classes to be generics. The array implementation should have dynamic resizing (double the size when growing and halve the size when less than 25 % of the capacity is used); and the linked list implementation should use <u>doubly linked</u> list. Also, the behavior of these methods should be equivalent to that of Java Standard Library’s classes ArrayList or LinkedList. Please refer to the corresponding descriptions online<a href="#_ftn2" name="_ftnref2"><sup>[2]</sup></a>/<a href="#_ftn3" name="_ftnref3"><sup>[3]</sup></a>.




For the rest of the methods of the List interface, you may just throw an exception:

public type someUnneededMethod() {

throw new UnsupportedOperationException();

}




Question 2:

<strong> </strong>

Write your driver class ListTester. Use both of your list implementations and compare them to the

corresponding Java library implementations ( <em>ArrayList</em> and <em>LinkedList</em>) For numbers <em>N </em>= {10, 100, 1000, 10000, 100000, 1000000}




<ol>

 <li>Starting with <em>empty </em>lists of Number-s; measure how long it takes to insert N integer numbers (int, or Integer) with random values ranging from 0 to 2N into the lists, when inserting them at the <em>beginning</em>, at the <em>end</em>, and into a <em>random location </em>of the list (use indices to indicate where to do the insertion (e.g., add (randomLocation, number)).</li>

</ol>




<ol>

 <li>Starting with <em>non-empty </em>lists of N items (e.g., from part <em>a</em>), measure how long it takes to remove N numbers from the lists when removing them from the beginning, from the end, and from a random location of the list (use indices to indicate the location).</li>

 <li>Starting with <em>non-empty </em>lists of N items (same as part <em>b</em>), measure how long it takes to remove N random numbers (with values between 0 and 2N) from the four lists (some values might not exist in the list!).</li>

</ol>




<ul>

 <li>Produce the following table (the timing values below are just an illustration and do not relate to any real measurements):</li>

</ul>

<table width="589">

 <tbody>

  <tr>

   <td width="121">N = 10</td>

   <td width="156"><strong><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="c78ea9b4a2b5b387">[email protected]</a></strong>start(ms)</td>

   <td width="144"><strong><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="2960475a4c5b5d69">[email protected]</a></strong>end (ms)</td>

   <td width="168"><strong><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="1851766b7d6a6c58">[email protected]</a></strong>random (ms)</td>

  </tr>

  <tr>

   <td width="121">MyArrayList</td>

   <td width="156">18</td>

   <td width="144">110</td>

   <td width="168">310</td>

  </tr>

  <tr>

   <td width="121">ArrayList</td>

   <td width="156">18</td>

   <td width="144">110</td>

   <td width="168">310</td>

  </tr>

  <tr>

   <td width="121">MyLinkedList</td>

   <td width="156">18</td>

   <td width="144">110</td>

   <td width="168">310</td>

  </tr>

  <tr>

   <td width="121">LinkedList</td>

   <td width="156">18</td>

   <td width="144">110</td>

   <td width="168">310</td>

  </tr>

 </tbody>

</table>




<table width="660">

 <tbody>

  <tr>

   <td width="102">N = 10</td>

   <td width="130"><strong><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="7123141c1e071431">[email protected]</a></strong>start(ms)</td>

   <td width="128"><strong><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="7725121a18011237">[email protected]</a></strong>end(ms)</td>

   <td width="144"><strong><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="de8cbbb3b1a8bb9e">[email protected]</a></strong>random(ms)</td>

   <td width="156"><strong>Remove </strong>byvalue (ms)</td>

  </tr>

  <tr>

   <td width="102">MyArrayList</td>

   <td width="130">10</td>

   <td width="128">150</td>

   <td width="144">200</td>

   <td width="156">1234567</td>

  </tr>

  <tr>

   <td width="102">ArrayList</td>

   <td width="130">10</td>

   <td width="128">150</td>

   <td width="144">200</td>

   <td width="156">1234567</td>

  </tr>

  <tr>

   <td width="102">MyLinkedList</td>

   <td width="130">10</td>

   <td width="128">150</td>

   <td width="144">200</td>

   <td width="156">1234567</td>

  </tr>

  <tr>

   <td width="102">LinkedList</td>

   <td width="130">10</td>

   <td width="128">150</td>

   <td width="144">200</td>

   <td width="156">1234567</td>

  </tr>

 </tbody>

</table>




<ul>

 <li>Repeat for all values of N = 100; N = 1000; …. etc.</li>

 <li>Save the result of your program execution in a file testrun.txt and submit it together with your other files.</li>

</ul>








