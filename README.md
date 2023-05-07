Download Link: https://assignmentchef.com/product/solved-homework-05-arrays
<br>
<h1>Prerequisites</h1>

<ol>

 <li>Arrays

  <ul>

   <li>Know how to declare, initialize and use multidimensional arrays.</li>

  </ul></li>

 <li>Repetition

  <ul>

   <li>Use loops to traverse through a multidimensional array.</li>

  </ul></li>

 <li>Scanner Libraries</li>

</ol>




<h1>Description</h1>

Arrays are data structures consisting of a collection of elements of the same type. Each element is accessible via 1 or more indices. In a one-dimensional array, each element can be accessed using one index. For example, arr[2]​ accesses the third element of the one-dimensional array called arr​ .​ In a two-dimensional array, each element can be accessed using two indices. For example, arr[2][1]​ accesses the element at the third row and the second column of a two-dimensional array called arr​ .​




To access all elements of an array, it is convenient to use for​ loops. For a one-dimensional array, the following will print all elements of the array called arr​ , one on each line:​




<strong>for (int i = 0; i &lt; arr.length; i++) { System.out.println(arr[i]); </strong>

<strong>} </strong>




And similarly for a two-dimensional array, one <strong>for</strong>​ loop for each dimension can be used:​




<strong>for (int i = 0; i &lt; garage.length; i++) { System.out.println(“Row: ” + i); </strong>

<strong>for (int j = 0; j &lt; garage[i].length; j++) { System.out.println(arr[i][j]); </strong>

<strong>} </strong>

<strong>System.out.println(); } </strong>




In this assignment you will be creating a simulation for Conway’s Game of Life. To see a simulation you can go to <u>​</u><u><a href="https://bitstorm.org/gameoflife/">https://bitstorm.org/gameoflife/</a></u><u>​</u><a href="https://bitstorm.org/gameoflife/">.</a> The general rules are as follows:




<strong>Rules: </strong>

<ul>

 <li><strong>For a cell that is ‘alive’ or ‘populated’:</strong></li>

 <li>Any cell with fewer than two live neighbors dies Any cell with more than three live neighbors dies ● Any cell with two or three neighbors survives.</li>

 <li><strong>For a cell that is ’empty’ or ‘unpopulated’: </strong></li>

 <li>Each cell with three neighbors becomes populated.</li>

</ul>




An empty cell will be denoted with a 0 whereas a populated cell will be shown as a 1.




<h1>Visual Example</h1>

<strong> </strong>

In these examples the black cells are live and the white cells are dead.




<strong>                              </strong>Generation 0                                 Generation 1​

<strong> </strong>

<h1>Tasks</h1>

<h2>Task 1 – Create the Initial Grid  (10 Points)</h2>

<ol>

 <li>At the beginning of the program, ask the user to enter one value for the size of the square matrix</li>

</ol>




<ol start="2">

 <li>Then create a two-dimensional array of ints​ to represent the grid . You can assume that t<strong>he user will input a valid integer</strong>​ .​</li>

</ol>




<ol start="3">

 <li>Have the user enter the strings that follow the form “0,1,0,1,1,0…,1” for each row.</li>

</ol>




<ol start="4">

 <li>Print out Generation 0: followed by the 2D array</li>

</ol>







Enter number of rows/columns:

<em>3 </em>




<em>1,0,1 </em>

<em>1,1,0 </em>

<em>0,1,1 </em>




Generation 0:

1 0 1

1 1 0

0 1 1

<h2>Task 2 – Calculating Next Generation (85 Points)</h2>

Using the Conway’s Game of Life Rules listed above, create the next generation of cells.

//after one iteration Generation 0 becomes Generation 1

Generation 0:

<ul>

 <li>1 1</li>

 <li>0 0</li>

</ul>

0 1 0




Generation 1:

<ul>

 <li>1 0</li>

 <li>0 1</li>

</ul>

0 0 0

<h2>Task 3 – Looping  (5 Points)</h2>

<ol>

 <li>If the user inputs “q” or “Q”, then the program will terminate</li>

</ol>




<ol start="2">

 <li>If the user inputs any character other than “q” or “Q”, the program will output the next generation of cells.</li>

</ol>

<h1>Example Execution</h1>

<table width="602">

 <tbody>

  <tr>

   <td width="602">Enter number of rows/columns: <em>3</em>​<em>0,1,1 </em><em>1,0,0 </em><em>0,1,0 </em> Generation 0:0  1 11  0 00 1 0<em>n </em>Generation 1:0  1 01  0 10 0 0<em>n </em>Generation 2:0 1 00 1 00 0 0<em>n </em>Generation 3:0 0 00 0 00 0 0<em>n </em>Generation 4:0 0 00 0 00 0 0<em>q </em>Program Terminated</td>

  </tr>

 </tbody>

</table>




<h2>Submission</h2>

Items needed for submission

<strong>– GameOfLife.java </strong>




<strong> </strong>