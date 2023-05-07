# Huffman-Algorithm
Huffman Coding is one of the lossless data compression techniques. It assigns variable-length codes to the input characters, based on the frequencies of their occurence. The most frequent character is given the smallest length code.

The variable-length codes assigned to input characters are Prefix Codes, means the codes (bit sequences) are assigned in such a way that the code assigned to one character is not the prefix of code assigned to any other character.

![image](https://user-images.githubusercontent.com/106259041/236661500-2fc30f4c-177c-4a58-be29-f19c03352bac.png)

### Process of Compression
<ul>
<li>Building frequency dictionary

<li>Select 2 minimum frequency symbols and merge them repeatedly: Used Min Heap

<li>Build a tree: Created a HeapNode class and used objects to maintain tree structure.

<li>Assign code to characters: Recursively traversed the tree and assigned the corresponding codes

<li>Encode the input text. Added padding to the encoded text, if it’s not of a length of multiple of 8. Stored this padding information, in 8 bits, in the beginning of the resultant code.

<li>Write the result to an output binary file, which will be our compressed file.
