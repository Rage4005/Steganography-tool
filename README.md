# Steganography-tool
Basic Steganography Tool

Overview

This project allows you to hide and extract secret messages within images using the Least Significant Bit (LSB) steganography technique.

Features

Encode secret messages into images.

Decode hidden messages from encoded images.

Supports common image formats (PNG, JPG, BMP).

Project Structure

Steganography-Tool/
├── steganography.py   # Core encoding/decoding logic
├── gui.py             # Optional GUI using Tkinter
├── README.md          # Project documentation
├── example_images/    # Sample images for testing
├── requirements.txt   # List of dependencies

Installation

Clone the repository:

git clone https://github.com/yourusername/Steganography-Tool.git
cd Steganography-Tool

Install required dependencies:

pip install -r requirements.txt

Usage

Encoding a message:

from steganography import encode_message

image_path = "example_images/input_image.png"
message = "Hidden secret message!"
output_path = "example_images/encoded_image.png"

encode_message(image_path, message, output_path)

Decoding a message:

from steganography import decode_message

encoded_image_path = "example_images/encoded_image.png"
decoded_message = decode_message(encoded_image_path)
print("Decoded message:", decoded_message)

Example Images

Place sample images in the example_images/ directory to test the tool.

Dependencies

The required Python libraries are listed in requirements.txt:

Pillow
NumPy

Future Improvements

Add encryption for enhanced security.

Implement a graphical user interface.

License

This project is licensed under the MIT License.

Author

Your Name - Your GitHub Profile

