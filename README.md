# csc347-ens211-lab-8--9-s-complementer-solved
**TO GET THIS SOLUTION VISIT:** [CSC347-ENS211 Lab 8 -9’s Complementer Solved](https://www.ankitcodinghub.com/product/csc347-ens211-lab-8-9s-complementer-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;94118&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSC347-ENS211 Lab 8 -9’s Complementer Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<h1>Lab 8 &nbsp;&nbsp;9’s Complementer</h1>
&nbsp;

<strong>Objective </strong>

The objective of this lab is to design a 9’s complementer from a hierarchy of components using Verilog description and simulate using a test bench.

&nbsp;

<strong>Lab Procedure</strong>

In this lab assignment, you will continue to practice hierarchical design by designing a 9’s complementer using verilog. You will start with the design from the previous lab (half adder and full adder), then build a 4-bit adder, 4-bit adder/subtractor, and finally a 9’s complementer.

&nbsp;

<ul>
<li>Half-adders in terms of gates. (Lab 7)</li>
<li>Full-adders in terms of half-adders (Lab 7)</li>
<li>4-bit adder in terms of full-adders</li>
<li>4-bit adder/subtractor in terms of 4-bit adder</li>
<li>9’s complementer in terms of 4-bit adder/subtractor</li>
</ul>
Like 2’s complement, 9’s complement is used to subtract a number using addition. 9’s complement of a decimal number is the subtraction of its each digit from 9. The block diagram of a 1-digit 9’s complementer is shown below. The input decimal digit (0 – 9) is represented as a 4-bit binary, and the output generates the 9’s complement in binary by calculating y = 9 – x.

<table>
<tbody>
<tr>
<td width="0"></td>
<td width="37"></td>
<td width="110"></td>
<td width="106"></td>
</tr>
<tr>
<td></td>
<td rowspan="2"></td>
</tr>
<tr>
<td></td>
<td></td>
<td rowspan="2"></td>
</tr>
<tr>
<td></td>
</tr>
</tbody>
</table>
&nbsp;

<ol>
<li>Copy your Lab 7’s verilog code for half adder and full adder (from “your playground” on EDAplayground.com).</li>
<li>Build a 4-bit adder: In this part, we will design a 4-bit adder following the topology of the circuit diagram. In the following module for the 4-bit adder, add Verilog statements below the comments so it matches the circuit. The module for 1-bit full adder from Lab 7 is “fulladder (S, C, x, y, cin)”</li>
</ol>
module four_bit_adder (S, C4, A, B, Cin);

input [3:0] A,B;

input Cin;

output [3:0] S;

output C4;

&nbsp;

&nbsp;

//Declare intermediate carries

wire C1, C2, C3;

&nbsp;

//Instantiate the fulladder

fulladder FA0(S[0], C1, A[0], B[0], Cin);

fulladder FA1(S[1], C2, A[1], B[1], C1);

fulladder FA2(S[2], C3, A[2], B[2], C2);

fulladder FA3(S[3], C4, A[3], B[3], C3);

&nbsp;

endmodule

&nbsp;

<ol start="3">
<li>Build a 4-bit adder/subtractor: Complete the following Verilog module so it matches the circuit below.</li>
</ol>
&nbsp;

module adder_subtractor(S, C, A, B, M);

input [3:0] A,B;

input M;

output [3:0] S;

output C;

&nbsp;

//Declare outputs of XOR gates

wire [3:0]N;

&nbsp;

// Instantiate the XOR gates

xor XOR0(N[0],B[0], M);

xor XOR1(N[1],B[1], M);

xor XOR2(N[2],B[2], M);

xor XOR3(N[3],B[3], M);

&nbsp;

// Declare carry

wire C4;

&nbsp;

// Instantiate the 4-bit full adder

four_bit_adder FBA(S, C4, A, N, M);

&nbsp;

endmodule

&nbsp;

&nbsp;

<ol start="4">
<li>Write a Verilog module for the 9’s complementer:</li>
</ol>
&nbsp;

module nine_s_complementer (x,y);

input [3:0] x;

output [3:0] y;

&nbsp;

// Declare wire

wire C4;

&nbsp;

// Instantiate the nine_s_complementer

adder_subtractor AS(y, C4, 9, x, 1);

endmodule

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</strong>

<ol start="5">
<li>Write a testbench program to test the 9’s complementer. Fill in the blanks and add all the test cases after the comment<strong> “</strong>// Initialize Inputs”</li>
</ol>
&nbsp;

<strong>&nbsp;</strong>

<strong>module test;</strong>

<strong>&nbsp; // input</strong>

<strong>&nbsp; reg[3:0] x; </strong>

<strong>&nbsp; // output</strong>

<strong>&nbsp; wire[3:0] y;&nbsp;&nbsp; </strong>

<strong>&nbsp;</strong>

<strong>&nbsp; // Instantiate the Unit Under Test (UUT)</strong>

<strong>&nbsp; nine_s_complementer uut(x,y);&nbsp; </strong>

<strong>&nbsp;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; initial </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; begin</strong>

<strong>$dumpfile(“dump.vcd”);&nbsp; $dumpvars(1, test);&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // display the inputs and outputs</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; $monitor( “x = %d&nbsp; y = %d”, x, y);</strong>

<strong>&nbsp;</strong>

<strong>&nbsp;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; // Initialize Inputs</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for(int i = 0; i &lt; 10; i = i + 1) begin</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; {x} = i;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end</strong>

<strong>&nbsp;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #10 $finish;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; endmodule&nbsp;&nbsp; </strong>

<strong>&nbsp;</strong>

&nbsp;

<ol start="6">
<li><strong>Test on EDAplayground.com</strong></li>
</ol>
<ul>
<li>Log into your EDAplayground.com account.</li>
<li>Edit your Verilog design code and testbench code in the right and left windows respectively, enter a name such as “Lab 9” for your project in the edit box at the bottom and click the “<u>Save</u><strong>” </strong>button to save your project.</li>
<li>On the left panel, under <u>Tools and Simulations</u>, select <u>Icarus Verilog 0.9.7</u> and check the box of “<u>Open <strong>EPwave</strong> after Run</u>”</li>
<li>Click “<u>Run</u>” at the top to run the simulation, watch for waveforms and verify your full adder works correctly.</li>
</ul>
<strong><u>&nbsp;</u></strong>

<strong><u>Submission Instructions:</u></strong>

<strong><u>&nbsp;</u></strong>

<u>Lab work submission</u>

<ol>
<li>Take a screenshot of your wavefroms.</li>
<li>Add the following information as comments to the beginning of your code. Make sure to click the “Save” button to save your project, then take a screenshot of your code.</li>
</ol>
// Author:&nbsp;&nbsp;&nbsp; Name

// Lab 8:&nbsp; put the title here

// Link to your project

&nbsp;

<ol start="3">
<li>Copy the link of your design from the address bar of the browser.</li>
<li>On the Blackboard, click on Lab 8. Attach the screenshot from the first two steps and paste the link from Step 3 into the Comments area, then click the “Submit” button.</li>
</ol>
&nbsp;

&nbsp;

<strong>You do not need to write a lab report for this lab but do the following homework and submit the screenshots and link to the Blackboard under Lab 8 report submission. </strong>It is due one week after the lab is done.

&nbsp;

<strong>Homework</strong>: write a Verilog deisgn code and testbench for implementing a 4-bit x 3-bit multiplier&nbsp;using 12 AND gates and two 4-bit adders shown in the diagram. You can use the 4-bit adder module from above. Test at least 10 input cases.

<strong>&nbsp;</strong>

<strong>module multiplier(</strong>C, A, B<strong>);&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; module </strong>test<strong>;</strong>

input [3:0] A;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;………

input [2:0] B;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;………

output [6:0] C;

………

………&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>en</strong><strong>dmodule</strong>

<strong>endmodule</strong>
