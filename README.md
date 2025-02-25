Secure Data Hiding in Image Using Steganography

1.Overview

This project implements image-based steganography to securely hide and extract secret messages within digital images. By using Least Significant Bit (LSB) encoding, the system ensures data confidentiality while keeping the cover image visually unchanged.

2.Features

Text Encryption & Decryption: Hide messages inside an image and retrieve them securely.

Password Protection: Ensures only authorized users can extract hidden data.

Minimal Image Distortion: Uses LSB technique for subtle modifications.

Supports Common Image Formats: Works with PNG, JPEG, and BMP.


3.Technologies Used

Programming Language: Python

Libraries: OpenCV, NumPy, PIL (Pillow)

Algorithms: Least Significant Bit (LSB) encoding


4.Installation

Prerequisites

Ensure you have Python installed. You can install required libraries using:

sudo apt update && sudo apt install python3 python3-pip -y

pip3 install opencv-python numpy pillow

Clone the Repository

git clone https://github.com/your-repository/steganography.git
cd steganography

5.Usage

Hiding a Message
   
   Run the script and provide an image and a secret message:

   python3 hide_message.py mypic.jpg "This is a secret message"
   
   The output will be encryptedImage.jpg with the hidden message.
   
Extracting a Message

To retrieve the hidden message:

python3 extract_message.py encryptedImage.jpg

Enter the passcode when prompted to decrypt the message.
    
6.Expected Output

Encrypted Image: An image that looks the same but contains hidden data.

Decrypted Message: The extracted secret text if the correct passcode is provided.

7.Limitations & Future Enhancements

Current implementation works best with smaller text messages.

Can be improved with AES encryption for stronger security.

Future versions may support video steganography.

8.Contributors- Ankit Pandey



