---
layout: page
title: 3rd Normal Form
---

## What exactly is 3nf?

Getting your tables to third normal form may seem easy enough--and it really isn’t _that_ complicated--but I have had to double and triple check during this semester. I think I understand and have properly implemented 3nf, but then again I’m not so sure. So, what is 3nf exactly?

Well, one part of being in 3nf is being in 2nf. And one part of being in 2nf is being in 1nf. Let’s start at 1nf.

A table is in First Normal Form if:
*   Each row of data contains <span style="text-decoration:underline;">atomic values</span>
    *   A table with atomic values can’t have multiple columns with the same type of data
   
    *   or several values of the same type of data in a single column

*   Each row of data has a unique identifier, known as a <span style="text-decoration:underline;">primary key</span>
    *   A primary key is a column in a table that makes each record unique

A table is in Second Normal Form if:
*	It is in 1nf
*	It has no <span style="text-decoration:underline;">functional dependencies</span>
    *   Basically, if all the columns in the table are part of the primary key (composite key) or if the table has a single column primary key

And finally, a table is in Third Normal Form if:
*	It is in 2nf
*	It has no <span style="text-decoration:underline;">transitive dependencies</span>
    *   Transitive dependencies occur when a non-key column is related to any of the other non-key columns, such that changing one of the non-key columns results in another column to change

Achieving 3nf in your tables really isn’t that confusing, at least not when you lay out all the requirements and make sure that you meet them.
