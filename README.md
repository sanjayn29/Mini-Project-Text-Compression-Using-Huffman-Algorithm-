# Huffman Text Compression

## Project Description
This project implements **Huffman Coding**, a lossless data compression algorithm. It compresses text by assigning variable-length binary codes to characters based on their frequency. Frequent characters are assigned shorter codes, reducing the overall size of the data. The program also includes decoding functionality to ensure the original text can be accurately reconstructed from the compressed data.

---

## Features
- **Text Compression**: Compresses input text into a binary format using Huffman Coding.
- **Text Decompression**: Decodes the compressed binary data back into the original text.
- **Huffman Code Generation**: Creates a mapping of characters to binary codes based on frequency.
- **Lossless Compression**: Ensures the original text can be perfectly reconstructed.

---

## Technologies Used
- **Python**: The core programming language for this project.
- **heapq**: Used for building the priority queue for the Huffman Tree.
- **collections.Counter**: To calculate character frequencies in the input text.

---

## How It Works
1. **Frequency Calculation**: Counts the frequency of each character in the input text.
2. **Huffman Tree Construction**: Builds a binary tree using a min-heap (priority queue).
3. **Code Generation**: Assigns binary codes to characters based on their position in the Huffman Tree.
4. **Encoding**: Replaces each character in the text with its Huffman code, producing compressed binary data.
5. **Decoding**: Traverses the Huffman Tree to convert the binary data back to the original text.

---

## Example Usage

### Input:
```plaintext
"huffman coding is a data compression algorithm"
```

### Output:
#### Huffman Codes:
```python
{'h': '1100', 'u': '1101', 'f': '1011', 'm': '100', 'a': '010', 'n': '011', ' ': '00', 'c': '1010', 'o': '1111', 'd': '1110', 'i': '0110', 's': '0100', 't': '0101', 'p': '0111', 'e': '1000', 'r': '1001', 'g': '1100', 'l': '1101'}
```
#### Encoded Text:
```plaintext
1100110110111010001011101011101011111100111010000010111111010011011111010010110110000100110001
```
#### Decoded Text:
```plaintext
"huffman coding is a data compression algorithm"
```

---

## Usage Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd huffman-text-compression
   ```

2. Run the Python script:
   ```bash
   python huffman_compression.py
   ```

3. Input your text to:
   - Generate Huffman codes for each character
   - Get the compressed (encoded) binary text
   - Verify the original text is accurately reconstructed through decoding

---

## 👨‍💻 Developer

**Sanjay N** 🚀 Freelancer

🌐 Portfolio: https://sanjayn.me  
💼 LinkedIn: https://linkedin.com/in/sanjayn29  
🐙 GitHub: https://github.com/sanjayn29  

---

## ⭐ Support

If you like this project, consider giving it a **star ⭐ on GitHub** to support the development.
