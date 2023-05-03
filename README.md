Download Link: https://assignmentchef.com/product/solved-cs-201-data-structures-library-phase-3
<br>



Phase 3 of the CS201 programming project, we will be built around heaps.  In particular, you should implement both a standard binary heap and binomial heap.  You will implement a class for each heap type.

You should create a class named Heap for the binary heap with public methods including the following (elmtype and valuetype are types from the template).  You should use your dynamic array class for the heap storage.

<table width="623">

 <tbody>

  <tr>

   <td width="228">Function</td>

   <td width="312">Description</td>

   <td width="84">Runtime</td>

  </tr>

  <tr>

   <td width="228">Heap();</td>

   <td width="312">Default Constructor. The Heap should be empty</td>

   <td width="84">O(1)</td>

  </tr>

  <tr>

   <td width="228">Heap(keytype k[], valuetype V[], int s);</td>

   <td width="312">For this constructor the heap should be built using the arrays K and V containing s items of keytype and valuetype.  The heap should be constructed using the O(n) bottom up heap building method.</td>

   <td width="84">O(s)</td>

  </tr>

  <tr>

   <td width="228">~Heap();</td>

   <td width="312">Destructor for the class.</td>

   <td width="84">O(1)</td>

  </tr>

  <tr>

   <td width="228">keytype peekKey();</td>

   <td width="312">Returns the minimum key in the heap without modifiying the heap.</td>

   <td width="84">O(1)</td>

  </tr>

  <tr>

   <td width="228">valuetype peekValue();</td>

   <td width="312">Returns the value associated with the minimum key in the heap without modifiying the heap.</td>

   <td width="84">O(1)</td>

  </tr>

  <tr>

   <td width="228">keytype extractMin();</td>

   <td width="312">Removes the minimum key in the heap and returns the key.</td>

   <td width="84">O(lg n)</td>

  </tr>

  <tr>

   <td width="228">void insert(keytype k, valuetype v);</td>

   <td width="312">Inserts the key k and value v pair into the heap.</td>

   <td width="84">O(lg n)</td>

  </tr>

  <tr>

   <td width="228">void printKey()</td>

   <td width="312">Writes the keys stored in the array, starting at the root.</td>

   <td width="84">O(n)</td>

  </tr>

 </tbody>

</table>




Your class should include proper memory management, including a destructor, a copy constructor, and a copy assignment operator.

You should create a class named BHeap for the binomial heap with public methods including the following (elmtype and valuetype are types from the template).  You should use dynamic allocation for the binomial trees.

<table width="623">

 <tbody>

  <tr>

   <td width="228">Function</td>

   <td width="312">Description</td>

   <td width="84">Runtime</td>

  </tr>

  <tr>

   <td width="228">BHeap();</td>

   <td width="312">Default Constructor. The Heap should be empty</td>

   <td width="84">O(1)</td>

  </tr>

  <tr>

   <td width="228">BHeap(keytype k[], valuetype V[], int s);</td>

   <td width="312">For this constructor the heap should be built using the arrays K and V containing s items of keytype and valuetype.  The heap should be constructed using repeated insertion.</td>

   <td width="84">O(s)</td>

  </tr>

  <tr>

   <td width="228">~BHeap();</td>

   <td width="312">Destructor for the class.</td>

   <td width="84">O(n)</td>

  </tr>

  <tr>

   <td width="228">keytype peekKey();</td>

   <td width="312">Returns the minimum key in the heap without modifiying the heap.</td>

   <td width="84">O(lg n)</td>

  </tr>

  <tr>

   <td width="228">valuetype peekValue();</td>

   <td width="312">Returns the value associated with the minimum key in the heap without modifiying the heap.</td>

   <td width="84">O(lg n)</td>

  </tr>

  <tr>

   <td width="228">keytype extractMin();</td>

   <td width="312">Removes the minimum key in the heap and returns the key.</td>

   <td width="84">O(lg n)</td>

  </tr>

  <tr>

   <td width="228">void insert(keytype k, valuetype v);</td>

   <td width="312">Inserts the key k and value v pair into the heap.</td>

   <td width="84">O(lg n)</td>

  </tr>

  <tr>

   <td width="228">void merge(BHeap&lt;keytype, valuetype&gt; &amp;H2);</td>

   <td width="312">Merges the H2 into the current heap</td>

   <td width="84">O(lg n)</td>

  </tr>

  <tr>

   <td width="228">void printKey()</td>

   <td width="312">Writes the keys stored in the heap, printing the smallest binomial tree first.  When printing a binomial tree, print the size of tree first and then use a modified preorder traversal of the tree.See the example below.</td>

   <td width="84">O(n)</td>

  </tr>

 </tbody>

</table>








