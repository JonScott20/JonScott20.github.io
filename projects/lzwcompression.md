---
layout: page
permalink: lzwcompression
---

**LZW Compression Encoder**
--------------

**Project Type:** School - CPE 357

**Language Used: C**

**Learning Objectives**

* Learn the Lempel–Ziv–Welch (LZW) compression algorithm
* Utilize dynamic byte-packet size in order to improve compression ratios
* Implement a trie data structure and recycling mechanism
* Meet performance and memory standards in comparison to the reference solution

In order to learn the **LZW algorithm**, I referred to the following resources and practiced their examples by hand.
* [Wikipedia - LZW](https://en.wikipedia.org/wiki/Lempel%E2%80%93Ziv%E2%80%93Welch)
* [LZW Data Compression](http://marknelson.us/1989/10/01/lzw-data-compression/)
* [LZW Revisited](http://marknelson.us/2011/11/08/lzw-revisited/)

**Dynamic Packet Size:**
The packets ranged in size from 9 bits to 15, which is different than the original algorithm that used only 12 bit sized packets. For this project, the encoder always began with 9 bit-sized packets. As the dictionary is built, the packet size is increased when the code specifying the target string can no longer be stored in the previous packet. For example, 512 cannot be stored in a 9-bit packet, 10 bits are required to represent 512.

**Trie Data Structure**

Resource: [Wikipedia - Trie](https://en.wikipedia.org/wiki/Trie)

The trie data structure enabled a dictionary to be built and store large strings without actually storing the large strings themselves. Instead, singular nodes representing a single ASCII character with references to other nodes were used to determine if a string was already defined within the dictionary. A base dictionary was used, consisting of the 256 ASCII defined characters. When recycling, the dictionary was completely reset to its base.

**Performance and Memory**

Please reach out to me individually if you would like to know how I met performance and memory standards. I don't want to give too much away about how to compete with the instructor solution.

**Important Note**

For the scope of this class project, only the encoding portion of the LZW algorithm was implemented. We did not implement the decoder.

----------

[Return to Course Work](https://jonscott20.github.io/course_work/)

[Return to Project Directory](https://jonscott20.github.io/project_directory/)
