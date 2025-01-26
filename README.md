**Image Steganography**
This project implements Image Steganography using OpenCV and Python. The program allows encoding a secret message into an image by altering the least significant bits (LSB) of the image pixels and decoding the message from the image.

**Project Overview**
The goal of this project is to encode secret messages into an image, making it invisible to the human eye but retrievable through a decoding process. It uses OpenCV for image manipulation and bitwise operations for embedding and extracting messages.

**Features**
**Encoding:** Hide a secret message within an image.
**Decoding:** Retrieve the hidden message from the image.
**Customizable:** Input your own image and secret message for encoding.
**Technologies Used**
Python: The main programming language for implementing the functionality.
OpenCV: Used for image processing (reading, writing, and manipulating image pixels).
Numpy: For handling image data as arrays.
**Setup**
**Prerequisites**
Ensure the following libraries are installed:

OpenCV: Used for reading, writing, and processing images.
Numpy: Used for handling pixel data as arrays.
Install dependencies using:
pip install opencv-python numpy
**Code Overview**
messageToBinary(): Converts a message into its binary representation.
hideData(): Encodes a secret message into the least significant bits (LSB) of the image pixels.
showData(): Decodes the hidden message from the image.
Steganography(): The main function that provides the option to either encode or decode a message.
Running the Program
To run the steganography program:

python lsb.py
**The program provides two options:**

Encode the data: Embed a secret message into an image.
Input the image filename and the secret message to encode.
The program will output the image with the encoded message.
Decode the data: Extract the hidden message from an encoded image.
Encoding Process
The user inputs the image file and secret message.
The program hides the message in the image's least significant bits.
A new image with the hidden message is saved.
Decoding Process
The user inputs the encoded image.
The program extracts the hidden message from the least significant bits of the image pixels.
The secret message is printed on the console.
Example
Encoding:

Image: input_image.png
Secret Message: "This is a secret message"
Output Image: encoded_image.png
Decoding:

Image: encoded_image.png
Decoded Message: "This is a secret message"
