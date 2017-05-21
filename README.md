# SoloAlgorithmsProject1
This project demonstrates my knowledge and mastery in Dynamic Programming and Recursion
Honors Algorithms Course - Russian Doll Reassembly 

There are n dolls in the row, each with an integer size. You need to reassemble the matryoshka
sets, knowing neither the number of sets nor the number of dolls in each set.
You know only that every complete set consists of dolls with consecutive sizes
from 1 to some number m, which may vary between the different sets.
When reassembling the sets, you must follow these rules:
• You can put a doll or a nested group of dolls only inside a larger doll.
• You can combine two groups of dolls only if they are adjacent in the row.
• Once a doll becomes a member of a group, it cannot be transferred to
another group or permanently separated from the group. It can be temporarily
separated only when combining two groups.
Your time is valuable, and you want to do this reassembly process as quickly
as possible. The only time-consuming part of this task is opening and subsequently
closing a doll, so you want to minimize how often you do this. For
example, the minimum number of openings (and subsequent closings) when
combining group [1, 2, 6] with the group [4] is two, since you have to open the
dolls with sizes 6 and 4. When combining group [1, 2, 5] with the group [3, 4],
you need to perform three openings.


Your goal will be to write a program to print out instructions for the reassembly
process so as to minimize the number of openings and closings that
need to be done. If it is not possible to reassemble the dolls at all, given the
ordering of the dolls in the row, then you will indicate so by returning a file
with a single 0 in it.
The input file dolls.txt will look as follows.
4
2
3
1
1
2
1
So a large doll of size 4 is on the far left, then a smaller 2 doll, then a 3, and so
on. The instructions will detail the sequence of merges that the dolls undergo
to put them back together. In this case, the file instructions.txt will be
4 2 3 1 1 2 1
4 2 1,3 1 2 1
4 1,2,3 1 2 1
1,2,3,4 1 2 1
1,2,3,4 1,2 1
There should be 5 total openings and closings in this case. From the first line
to the second is one opening. From the second to the third is 2. From the third
to the fourth is 1, and the final is 1
