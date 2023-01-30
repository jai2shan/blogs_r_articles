<h2 style="text-align:center"> Testing Techniques </h2>


### 1) Orthogonal array Testing
* Orthogonal array testing is a black box testing technique that is a systematic, statistical way of software testing.    
* It is used when the number of inputs to the system is relatively small, but too large to allow for exhaustive testing of every possible input to the systems

Example :

<center>

Possible Values for each field

<table class="wikitable">

<tbody><tr>
<th>Parameter name</th>
<th>Value 1</th>
<th>Value 2</th>
<th>Value 3</th>
<th>Value 4
</th></tr>
<tr>
<td>Enabled</td>
<td>True</td>
<td>False</td>
<td>-</td>
<td>-
</td></tr>
<tr>
<td>Choice type</td>
<td>1</td>
<td>2</td>
<td>3</td>
<td>-
</td></tr>
<tr>
<td>Category</td>
<td>a</td>
<td>b</td>
<td>c</td>
<td>d
</td></tr></tbody></table>

Total Possible combinations for testing

<table class="wikitable">
<thead><tr>
<th >Enabled</th>
<th >Choice type</th>
<th >Category
</th></tr></thead><tbody>
<tr>
<td>True</td>
<td>3</td>
<td>a
</td></tr>
<tr>
<td>True</td>
<td>1</td>
<td>d
</td></tr>
<tr>
<td>False</td>
<td>1</td>
<td>c
</td></tr>
<tr>
<td>False</td>
<td>2</td>
<td>d
</td></tr>
<tr>
<td>True</td>
<td>2</td>
<td>c
</td></tr>
<tr>
<td>False</td>
<td>2</td>
<td>a
</td></tr>
<tr>
<td>False</td>
<td>1</td>
<td>a
</td></tr>
<tr>
<td>False</td>
<td>3</td>
<td>b
</td></tr>
<tr>
<td>True</td>
<td>2</td>
<td>b
</td></tr>
<tr>
<td>True</td>
<td>3</td>
<td>d
</td></tr>
<tr>
<td>False</td>
<td>3</td>
<td>c
</td></tr>
<tr>
<td>True</td>
<td>1</td>
<td>b
</td></tr></tbody><tfoot></tfoot></table>
</center>

**Source :**  
**https://en.wikipedia.org/wiki/Orthogonal_array_testing**   
**https://en.wikipedia.org/wiki/All-pairs_testing**  

### 2) Boundary Value Testing
Boundary value testing is the process of testing between extreme ends or boundaries between partitions of the input values.  
* So these extreme ends like Start- End, Lower- Upper, Maximum-Minimum, Just Inside-Just Outside values are called boundary values and the testing is called “boundary testing”.

![Boundary Value Testing](./images/testing_techniques/boundary_value_testing.png)

* The basic idea in normal boundary value testing is to select input variable values at their:  
        1) Minimum   
        2) Just above the minimum   
        3) A nominal value   
        4) Just below the maximum   
        5) Maximum  

### 2.1) Equivalence Partitioning
In this technique, input data units are divided into equivalent partitions that can be used to derive test cases which reduces time required for testing because of small number of test cases.    

Example 1: Equivalence and Boundary Value
Let’s consider the behavior of Order Pizza Text Box Below
Pizza values 1 to 10 is considered valid. A success message is shown.
While value 11 to 99 are considered invalid for order and an error message will appear, “Only 10 Pizza can be ordered”

Here is the test condition
1) Any Number greater than 10 entered in the Order Pizza field(let say 11) is considered invalid.       
2) Any Number less than 1 that is 0 or below, then it is considered invalid.        
3) Numbers 1 to 10 are considered valid         
4) Any 3 Digit Number say -100 is invalid.          

**Source : https://www.guru99.com/equivalence-partitioning-boundary-value-analysis.html**
### 3) Integration Testing
Integration testing -- also known as integration and testing (I&T) -- is a type of software testing in which the different units, modules or components of a software application are tested as a combined entity.

Example : 
1) Integration between DB and Application.    
> Should test scearios, of how data is saving  
2) Accessing data from API and displaying them in application

### 4) Unit testing

Writing Tests vs. Writing Code
**Source : https://www.makeuseof.com/testing-methods-developers-should-know/**