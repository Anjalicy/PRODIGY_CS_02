# Image Encryption Tool using Pixel Manipulation

This project implements a simple image encryption and decryption tool using pixel manipulation in Python. The tool performs encryption by applying a bitwise XOR operation on each pixel of the image with a user-provided numeric key. The same key is used for both encryption and decryption.

## Features
- Encrypts images by scrambling pixel values.
- Decrypts encrypted images using the same key.
- Simple and lightweight implementation using Python.
- Works with common image formats like PNG, JPG, etc.

## Requirements

Before running the tool, make sure you have the following libraries installed:

- `Pillow`: A Python Imaging Library to handle image processing.
- `numpy`: A library for efficient numerical operations.

You can install them using the following commands:

    pip install pillow numpy
    
# Usage

  1.Clone the repository or download the script.

  2.Run the script:

    python image_encrypt_decrypt.py

  3.Enter the path of the image you want to encrypt or decrypt.

  4.Enter the output path where you want to save the encrypted or decrypted image.

  5.Provide a numeric key (0-255) for encryption or decryption.

  6.Choose whether you want to encrypt or decrypt the image by entering e for encryption or d for decryption.

## Example

    Enter the path of the image: input_image.png
    Enter the output path for the encrypted/decrypted image: encrypted_image.png
    Enter a numeric key (0-255): 123
    Do you want to encrypt or decrypt the image? (e/d): e
    Encrypting the image...
    Image saved at: encrypted_image.png

# To decrypt the image, use the same numeric key:

    Enter the path of the image: encrypted_image.png
    Enter the output path for the encrypted/decrypted image: decrypted_image.png
    Enter a numeric key (0-255): 123
    Do you want to encrypt or decrypt the image? (e/d): d
    Decrypting the image...
    Image saved at: decrypted_image.png
# How It Works

  1.The image is loaded using Pillow and converted into a NumPy array to allow pixel manipulation.
  2.Each pixel in the image is processed using the bitwise XOR (^) operation with the user-provided key.
  3.The encrypted/decrypted image is saved to the specified output path.
  
## License

This project is licensed under the MIT License. See the LICENSE file for details.


