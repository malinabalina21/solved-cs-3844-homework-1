Download Link: https://assignmentchef.com/product/solved-cs-3844-homework-1
<br>
Homework #1 – Binary / Octal / Decimal / Unsigned / Hex

CS 3844 Section 0B1,

Write a C program that takes one or more numbers on the command line. Rules:

<ul>

 <li>If no numbers are given, print a usage message and quit.</li>

 <li>Do NOT use sscanf or similar. Process each argument one digit at a time.</li>

 <li>For each number given on the command line, check to see if it is a valid binary, octal, decimal and hex number. For hex numbers, allow both lowercase a-f and uppercase A-F.</li>

 <li>If there are any invalid characters in the argument, ignore it. E.g., a 2 is not valid for binary.</li>

 <li>You must also account for a leading minus sign. Additional error checking is not necessary (overflow for example).</li>

</ul>

Example usage: <strong>./hw1 0 123 abcd -45 error -1 -4D</strong>

Example output:

<strong>=== Checking 0               Octal      Decimal     Unsigned          Hex</strong>

<strong>Base  2:                         0            0            0            0</strong>

<strong>Base  8:                         0            0            0            0</strong>

<strong>Base 10:                         0            0            0            0</strong>

<strong>Base 16:                         0            0            0            0</strong>

<strong> </strong>

<strong>=== Checking 123             Octal      Decimal     Unsigned          Hex</strong>

<strong>Base  8:                       123           83           83           53</strong>

<strong>Base 10:                       173          123          123           7b</strong>

<strong>Base 16:                       443          291          291          123</strong>

<strong> </strong>

<strong>=== Checking abcd            Octal      Decimal     Unsigned          Hex</strong>

<strong>Base 16:                    125715        43981        43981         abcd</strong>

<strong> </strong>

<strong>=== Checking -45             Octal      Decimal     Unsigned          Hex</strong>

<strong>Base  8:               37777777733          -37   4294967259     ffffffdb</strong>

<strong>Base 10:               37777777723          -45   4294967251     ffffffd3</strong>

<strong>Base 16:               37777777673          -69   4294967227     ffffffbb</strong>

<strong> </strong>

<strong>=== Checking error           Octal      Decimal     Unsigned          Hex</strong>

<strong> </strong>

<strong>=== Checking -1              Octal      Decimal     Unsigned          Hex</strong>

<strong>Base  2:               37777777777           -1   4294967295     ffffffff</strong>

<strong>Base  8:               37777777777           -1   4294967295     ffffffff</strong>

<strong>Base 10:               37777777777           -1   4294967295     ffffffff</strong>

<strong>Base 16:               37777777777           -1   4294967295     ffffffff</strong>

<strong> </strong>

<strong>=== Checking -4D             Octal      Decimal     Unsigned          Hex</strong>

<strong>Base 16:               37777777663          -77   4294967219     ffffffb3</strong>

The columns must line up exactly as shown, but the number of spaces between columns doesn’t matter.

Hint: in C, printf with %-10s will left justify a string in 10 characters, %10s will right justify it.