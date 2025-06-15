Image Steganography Tool (GUI-based)

This project is a simple GUI-based Image Steganography tool built with Python. It allows you to encode (hide) secret messages inside an image and decode them later.

 Features
Encode Text into an Image
Hides any text data inside an image using Least Significant Bit (LSB) steganography.

Decode Text from an Image
Extracts the hidden message from a previously encoded image.

User-Friendly Interface
GUI built with Tkinter for easy interaction.

Tools & Technologies Used
Python 3.x

Tkinter – GUI framework

Pillow (PIL) – For image processing

 How It Works
 Encoding:
Each character of the secret message is converted to 8-bit binary.

These bits are embedded into the least significant bits of the RGB values of the image pixels.

The last bit in the pixel block marks the end of the message.

 Decoding:
The tool reads the LSBs of image pixels.

It reconstructs the binary sequence to characters.

It stops when the end marker bit is detected.

1 How to Run
Install Dependencies:

pip install pillow

2 Run the Application:

python main.py

3 Use the GUI to:

Choose an image path.

Enter the text to encode.

Set the output image name.

Encode or decode images as needed.


File Structure
main.py – Contains all functionality:

GUI setup

Encoding logic

Decoding logic

 Example Use Cases
Hide secret messages in images before sharing online.

Basic demonstration for cryptography or security-related educational projects.

Limitations
Works only with .png images.

Cannot encode large texts in small images (limited by pixel count).

No password protection or encryption – basic steganography only.

License
This project is open-source and free to use for educational purposes.
