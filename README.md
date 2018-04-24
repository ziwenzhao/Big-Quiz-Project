# Big-Quiz-Project
As you probably know, the “kloc” part of “Klocwork” stands for “thousands of lines of code”.  In this case, the task is easier:  count the millions of words on a single line.

 

Start with the definition of the following function:

 

Kw(integer n) =

    if n equals 0

        output “kloc”

    if n equals 1

       output “work”

    if n greater than 1

       output Kw(n-1) concatenated with Kw(n-2)

 

The output of this function for the first few values is:

 

Kw(0): "kloc"

Kw(1): "work"

Kw(2): "workkloc"

Kw(3): "workklocwork"

Kw(4): "workklocworkworkkloc"

Kw(5): "workklocworkworkklocworkklocwork"

Kw(6): "workklocworkworkklocworkklocworkworkklocworkworkkloc"

 

Your task is to write a program taking input of the value for n and a sub-string, and produce a count of the number of times that the sub-string occurs in Kw(n).

 

Input:

-          Input value for n; n shall be in the range of 0 <= n <= 100.

-          Input value for search string; string shall be non-empty with no spaces and a length of less than 100,000 characters.

 

Output:

-          Display the number of times that the sub-string appears in Kw(n).

-          The test guarantees that the answer is less than 2^63.

 

Note:

-          Occurrences of the sub-string may overlap.

 

Examples:

 

Input: 0 k

Output: 1

 

Input: 0 work

Output: 0

 

Input: 3 klocwork

Output: 1

 

Input: 6 workklocwork

Output: 4

 

Input: 30 kk

Output: 514229
 
get the results for  "40 klocwork" and "50 workklocwork".

The challenge is Fibonacci String is very long when n gets large, and the heap space is not enough to store it, so I have to think of other ways to solve the problems in space constraint.
