

# Encryption Techniques in Python

This project explores various classical and modern encryption techniques implemented in Python. Each notebook demonstrates a different cipher, showcasing how encryption algorithms transform data to enhance security. This collection of notebooks serves as a practical reference for anyone interested in learning encryption basics and implementing these methods.

## Project Overview

Encryption is essential for securing information. This project covers a range of encryption techniques, each with a unique approach to securing data. The notebooks include:
- **Classical Ciphers**: Caesar, Columnar, Vernam, Vigenère.
- **Modern Cipher**: AES (Advanced Encryption Standard).

## Project Structure

- **AES_Cipher.ipynb**: Implementation of the AES encryption algorithm, a widely used modern encryption technique for securing sensitive data.
- **Columnar_cipher.ipynb**: Demonstrates the columnar transposition cipher, a method that rearranges characters in a grid format.
- **Caesar_cipher.ipynb**: Illustrates the Caesar cipher, a basic substitution cipher where each letter is shifted a fixed number of positions.
- **Encryptions.ipynb**: Contains code for various encryption techniques.
- **Vernam.ipynb**: Showcases the Vernam cipher, also known as the one-time pad, a theoretically unbreakable encryption method.
- **Vigenere.ipynb**: Explains the Vigenère cipher, a polyalphabetic substitution cipher using a keyword.

## Technologies Used

- **Python**: All encryption techniques are implemented in Python.
- **Jupyter Notebooks**: Interactive environment for step-by-step code execution and explanations.

## Getting Started

1. **Environment Setup**: Make sure you have Python and Jupyter Notebook installed.
2. **Running Notebooks**: Open each `.ipynb` file in Jupyter Notebook to explore each encryption technique.

   ```bash
   pip install jupyter
   jupyter notebook
   ```

## How to Use

Each notebook includes code cells for the encryption and decryption processes. You can modify the input text or parameters (like keys and shifts) to see how they affect the output.

### Example Code Snippet (Caesar Cipher)

```python
def caesar_cipher(text, shift):
    result = ""
    for char in text:
        if char.isalpha():
            shift_base = ord('a') if char.islower() else ord('A')
            result += chr((ord(char) - shift_base + shift) % 26 + shift_base)
        else:
            result += char
    return result

encrypted_text = caesar_cipher("hello", 3)
print("Encrypted:", encrypted_text)
```

## Future Enhancements

- **Add More Ciphers**: Extend the project with additional modern encryption methods like RSA and DES.
- **Visualize Encryption Process**: Create visualizations to demonstrate how data is transformed during encryption and decryption.
- **Integrate with Applications**: Showcase practical applications by integrating these ciphers into small security-related projects.

## Contact

For questions or feedback, please reach out via email: anashssn@gmail.com
