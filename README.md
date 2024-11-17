Features

    Compression: Converts a string into a compact binary format with an accompanying encoding map.
    Decompression: Reconstructs the original string using the encoding map and binary data.
    Handles edge cases such as:
        Empty strings.
        Strings with a single unique character.
    Includes robust error handling for malformed inputs.

How It Works

    Huffman Encoding:
        Analyzes the frequency of characters in the input string.
        Builds a Huffman Tree to assign variable-length binary codes to characters.
        Outputs a compressed representation including the encoding map and binary data.

    Decompression:
        Reconstructs the Huffman Tree from the encoding map.
        Decodes the binary data to retrieve the original string.

Usage
Compress a String

Run the program and choose the compression option:

Enter the string to compress: aaaabbbcc
Compressed output:
a:0;b:10;c:11;
0000101011

Decompress a String

Provide the encoding map and binary data:

Enter the encoding map: a:0;b:10;c:11;
Enter the binary data: 0000101011
Decompressed output:
aaaabbbcc
