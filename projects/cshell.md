---
layout: page
permalink: cshell
---

**C Shell**
--------------

**Project Type:** School - CPE 357

**Language Used:** C

**Learning Objectives**

* Launch multiple processes sequentially from within a bare bones Unix shell implementation
* Create a I/O pipeline between processes by connecting the standard output of one process to the standard input of the next
* Support redirection from files for both input and output

**Example Command:** 
cat input.txt | sort -rn | uniq -c | head -10

**Hardest Part**

The hardest part was keeping track of which pipe file descriptors were open in the parent and all child processes. If a descriptor was open when it wasn't supposed to be, the pipeline would not execute properly.

---------

[Return to CPE 357](https://jonscott20.github.io/cpe357/)

[Return to Project Directory](https://jonscott20.github.io/project_directory/)
