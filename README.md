# Merkle–Hellman Knapsack Cipher

Educational implementation of the Merkle–Hellman knapsack cryptosystem in C.

## About

This project demonstrates how text encryption and decryption can be performed using the Merkle–Hellman knapsack cryptosystem. The program converts an input message into binary form, generates private and public keys, encrypts the message, and then restores the original text.

## Features

* Converts input text characters to binary representation
* Generates a superincreasing private key sequence
* Generates public key values using modular arithmetic
* Calculates the modular inverse using the extended Euclidean algorithm
* Encrypts text with the public key
* Decrypts ciphertext using the private key
* Displays intermediate values: keys, ciphertext, decrypted binary data, and restored text

## Project Structure

```text
.
├── 1OIB/
│   ├── main.c
│   ├── 1OIB.vcxproj
│   └── 1OIB.vcxproj.filters
├── 1OIB.sln
├── .gitignore
└── .gitattributes
```

## How It Works

The Merkle–Hellman cryptosystem is based on the subset sum problem.

The program performs the following steps:

1. Reads a text message from the user.
2. Converts each character into an 8-bit binary representation.
3. Generates a private superincreasing sequence.
4. Generates a modulus and multiplier.
5. Builds the public key.
6. Encrypts each binary block using the public key.
7. Uses the modular inverse to decrypt the ciphertext.
8. Restores the original text from binary form.

## Build and Run

### Using Visual Studio

1. Open `1OIB.sln`.
2. Build the solution.
3. Run the project.

### Using GCC

```bash
gcc 1OIB/main.c -o merkle_hellman
./merkle_hellman
```

## Example

```text
Enter the message: hello
```

The program outputs generated keys, encrypted values, decrypted binary blocks, and the restored text.

## Educational Purpose

This repository was created as a study project for learning basic concepts of information security, public-key cryptography, modular arithmetic, and the knapsack cryptosystem.
