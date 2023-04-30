Download Link: https://assignmentchef.com/product/solved-metcs526-module-2-analyzing-running-times-of-algorithms
<br>
<strong>Problem 1 </strong>. This problem is a practice of analyzing running times of algorithms. Express the running time of the following methods, which are written in a pseudocode style, using the <em>big-oh</em> notation. Assume that all variables are appropriately declared. You must justify your answers. If you show only answers, you will not get any credit even though they are correct.




(1)

method1(int[ ] a)  // returns integer

<ul>

 <li>= 0;</li>

 <li>= 0;</li>

</ul>

for (i=1; i&lt;n; i++) { // n is the number of elements in array <em>a </em>

if (a[i] == a[i‐1]) {

<ul>

 <li>= x + 1;</li>

</ul>

}

else {

<ul>

 <li>= y + 1;</li>

</ul>

}

}

return (x ‐ y);







(2)

method2(int[ ] a, int[ ] b)  // assume equal‐length arrays

x = 0;

<ul>

 <li>= 0;</li>

</ul>

while (i &lt; n) { // n is the number of elements in each array

y = 0;

<ul>

 <li>= 0;</li>

</ul>

while (j &lt; n) {

<ul>

 <li>= 0</li>

</ul>

while (k &lt;= j) {

y = y + a[k];

k = k + 1;

}

j = j + 1;

}

if (b[i] == y) {

x++;

} i = i + 1;

}

return x;




(3)




// <em>n</em> is the length of array <em>a</em>

// <em>p</em> is an array of integers of length 2

// initial call: method3(<em>a, n-</em>1<em>, p</em>)

// initially <em>p</em>[0] = 0, <em>p</em>[1] = 0

method3(int[] a, int i, int[] p)

if (i == 0) {

p[0] = a[0];

p[1] = a[0];

}

else {

method3(a, i‐1, p);

if (a[i] &lt; p[0]]) {

p[0] = a[i];

}

if (a[i] &gt; p[1]]) {

p[1] = a[i];

}




}




(4)




// initial call: method4(<em>a</em>, 0, <em>n</em>‐1) // <em>n</em> is the length of array <em>a</em> public static int method4(int[] a, int x, int y)  if (x &gt;= y) {return a[x];} else {  z = (x + y) / 2; // integer division u = method4(a, x, z);

v = method4(a, z+1, y);

if (u &lt; v) return u;

else return v;

}

}




<strong>Problem 2 (20 points).</strong>  This problem is a practice of drawing recursion traces of recursive algorithms.

<ul>

 <li>Draw the recursion trace for the computation of power(3, 4) using the algorithm of Code</li>

</ul>

Fragment 5.8.

<ul>

 <li>Draw the recursion trace for the computation of power(3, 14) using the algorithm of Code Fragment 5.9.</li>

</ul>

Examples of recursion traces are shown in Figure 5.10 and Figure 5.12. You may want to use these examples as models when you draw recursion traces.

<strong>Problem 3 </strong> This problem is about the stack and the queue data structures that is described in the textbook.

<ul>

 <li>Suppose that you execute the following sequence of operations on an initially empty stack. Using Example 6.3 as a model, complete the following table.</li>

</ul>




<table width="546">

 <tbody>

  <tr>

   <td width="84">Operation</td>

   <td width="114">Return Value</td>

   <td width="348">Stack Contents</td>

  </tr>

  <tr>

   <td width="84">push(10)</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="84">pop( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="84">push(12)</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="84">push(20 )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="84">size( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="84">push(7 )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="84">pop( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="84">top( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="84">pop( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="84">pop( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="84">push(35)</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="84">isEmpty( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

 </tbody>

</table>







<ul>

 <li>Suppose that you execute the following sequence of operations on an initially empty queue. Using Example 6.4 as a model, complete the following table.</li>

</ul>




<table width="560">

 <tbody>

  <tr>

   <td width="98">Operation</td>

   <td width="114">Return Value</td>

   <td width="348">Queue Contents (first ← Q ← last)</td>

  </tr>

  <tr>

   <td width="98">enqueue(7)</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="98">dequeue( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="98">enqueue(15)</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="98">enqueue(3 )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="98">first( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="98">dequeue( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="98">dequeue( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="98">first( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="98">enqueue(11 )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="98">dequeue( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="98">isEmpty( )</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

  <tr>

   <td width="98">enqueuer(5)</td>

   <td width="114"> </td>

   <td width="348"> </td>

  </tr>

 </tbody>

</table>




<strong>Problem 4 (40 points)</strong> This problem is a practice of designing and implementing small recursive methods. Write a program named <em>Hw2_P4.java</em> that includes two recursive methods.




The first method to be implemented is <em>reverseFirstN</em>, whose behavior is described below:




<ul>

 <li>This method receives two arguments, an integer array <em>a</em> and an integer <em>n</em>.</li>

 <li>It reverses order of the first <em>n</em> elements in the given array <em>a</em>.  This method must be a <strong><em>recursive</em></strong></li>

 <li>The signature of the method must be:</li>

</ul>




public static void reverseFirstN(int[] a, int n)

<ul>

 <li>You may want to write a separate method with additional parameters (refer to page 214 of the textbook).</li>

 <li>You may not use an additional array and the rearrangement of integers must occur within the given array <em>a</em>.</li>

</ul>




The second method to be implemented is <em>evenBeforeOdd</em> and its behavior is described below:




<ul>

 <li>This method receives one argument, an array of integers <em>a</em>.</li>

 <li>It rearranges the order of integers in <em>a</em> in such a way that all even integers come before all odd integers.</li>

 <li>The order of integers in the result is not important.  This method must be a <strong><em>recursive</em></strong></li>

 <li>The signature of the method must be</li>

</ul>




public static void evenBeforeOdd(int[] a)




<ul>

 <li>You may want to write a separate method with additional parameters (refer to page 214 of the textbook).</li>

 <li>You may not use an additional array and the rearrangement of integers must occur within the given array <em>a</em>.</li>

</ul>




<ul>

 <li>The following is an example of an input array and the rearranged array of the method:</li>

</ul>




Initial array: [10, 15, 20, 30, 25, 35, 40, 45]

After rearrange: [40, 10, 30, 20, 25, 35, 15, 45]




In the <em>Hw2_P4.java</em> program, write a main method to test the above two recursive methods. A sample test code segment is included in an incomplete <em>Hw2_P4.java</em> program posted on Blackboard. You must complete this program.




<strong>Deliverable</strong>




No separate documentation is needed for the program problem. However, you must include the following in your source code:

<ul>

 <li>Include the following comments above each method:</li>

 <li>Brief description of the method</li>

 <li>Input arguments</li>

 <li>Output arguments</li>

 <li>Include inline comments within your source code to increase readability of your code and to help readers better understand your code.</li>

</ul>




You must submit the following files:

<ul>

 <li><em>pdf</em>. This file must include the answers to problems 1, 2, and 3.  <em>Hw2_P4.java </em></li>

</ul>

<em> </em>

Combine all files into a single archive file and name it <em>LastName_FirstName_hw2.EXT</em>, where <em>EXT</em> is an appropriate archive file extension, such as <em>zip</em> or <em>rar</em>.




<strong> </strong>