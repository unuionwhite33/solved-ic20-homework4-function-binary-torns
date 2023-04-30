Download Link: https://assignmentchef.com/product/solved-ic20-homework4-function-binary-torns
<br>
<strong>Exercise 1 </strong>

Write the <strong>function</strong> <strong>binary-toRNS</strong> that:

<ul>

 <li>takes a radix-10 number X and a natural number n as <strong>input</strong></li>

 <li>computes the dynamic range M for the module set &lt; m<sub>1</sub>=2<sup>n</sup> -1 ; m<sub>2</sub>=2<sup>n</sup> ; m<sub>3</sub>= 2<sup>n</sup>+1 &gt; – computes the RNS representation &lt; x<sub>1</sub> x<sub>2</sub> x<sub>3</sub> &gt; of X for the module set &lt; m<sub>1</sub>=2<sup>n</sup> -1 ; m<sub>2</sub>=2<sup>n</sup> ; m<sub>3</sub>= 2<sup>n</sup>+1 &gt;</li>

 <li>gives as <strong>output</strong> the dynamic range M and the triple &lt; x<sub>1</sub> x<sub>2</sub> x<sub>3</sub> &gt;</li>

</ul>

Write the <strong>function</strong> <strong>Radix10-toRB</strong> that:

<ul>

 <li>takes radix-10 number D as <strong>input</strong></li>

 <li>computes the RB representation of D in canonical form as two binary strings N and R, one for normal bits and one for redundant bits</li>

 <li>gives as <strong>output</strong> the two binary strings N and R representing D</li>

</ul>

Write the <strong>function</strong> <strong>RB-toRadix10</strong> that:

<ul>

 <li>takes two binary strings N and R representing an RB number as <strong>input</strong></li>

 <li>computes the radix-10 associated value X</li>

 <li>gives as <strong>output</strong> either X or an error message if an overflow occurs (<em>with respect to</em> <em>the representation range corresponding to the number of bit considered) </em></li>

</ul>

Write the <strong>function</strong> <strong>RB-Sum </strong>that:

<ul>

 <li>takes two RB numbers <strong>A and B</strong> as <strong>input </strong></li>

 <li>computes the sum S applying the RB table</li>

 <li>gives as output S in RB representation</li>

</ul>




Write a script calling the functions above to compute the sum among a pairs of numbers randomly chosen in the range [0, M-1], where M is the dynamic range for the RNS representation with respect to a given n and module set &lt; m<sub>1</sub>=2<sup>n</sup> -1 ; m<sub>2</sub>=2<sup>n</sup> ; m<sub>3</sub>= 2<sup>n</sup>+1 &gt;.

The script shows: i) The two random values X1 and X2, ii) the RNS representation of X1 and X2 and of the sum S=X1+X2, iii) the strings obtained with the two steps of the RB sum for the three digits of the RNS representation.




<strong>Exercise 2 </strong>

Compute the <strong>time </strong>and<strong> area</strong> <strong>speedup</strong> with respect to a standard binary execution using a ripplecarry adder, when computing the sum among the K pairs of numbers randomly chosen in the range [0, M-1], (where M is the dynamic range for the RNS representation with respect to a given n and module set &lt; m<sub>1</sub>=2<sup>n</sup> -1 ; m<sub>2</sub>=2<sup>n</sup> ; m<sub>3</sub>= 2<sup>n</sup>+1 &gt;) in the following cases:

<ul>

 <li>Pipelined addition using an array adder for binary values</li>

 <li>RNS values with digits represented in binary and sum executed through ripple-carry adders for the single digits</li>

 <li>RNS values with digits represented in RB and sum executed through application of the RB table, taking into account that the application of the table corresponds to the circuit in the picture.</li>

</ul>

Show the results in two graphs: a first graph where n takes values 3, 4 and 5, and a second graph where K takes values 100, 500, 1000 (or more).

<strong><em>Remark</em></strong><em> This exercise requires only the computation of values, not the simulation of execution of the operations. </em>