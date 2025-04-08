# CryptМе

CryptМе is a video steganography tool that embeds arbitrary files into video content, employing metadata encryption for enhanced security.

## Description

CryptМе offers a method for concealing data within video files by combining steganography with cryptography. A distinctive aspect of this approach is the encryption of metadata (such as the file size, CRC, and markers) before embedding them into the video—a method that, based on current research, is not commonly implemented in existing solutions.

## Features

- **Metadata Encryption:**  
  Prior to embedding, metadata is encrypted using AES (ECB mode) to add an extra layer of security.
  
- **Data Embedding in Video:**  
  Utilizes LSB (Least Significant Bit) steganography to hide data within the pixel values of video frames.
  
- **Pseudo-Random Distribution:**  
  Embedding positions are determined pseudo-randomly using an AES-based PRNG, making detection of the hidden information much harder.

## Technologies Used

- **OpenCV:** For video frame processing.
- **NumPy:** For data manipulation and bit-level operations.
- **PyCryptodome:** For AES encryption.

## Requirements

- Python 3.x
- OpenCV
- NumPy
- PyCryptodome

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/CryptMe.git
