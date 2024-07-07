

# Aadhaar UID Masking Tool

This project provides support of Extraction, Veriﬁcation and Masking of Aadhaar UIDs from photos and scanned documents. The solution to the problem involves use of PyTesseract a Optical Character Recognition engine and OpenCV for image processing. 

# Abstract
Identity theft and scams are major concerns in today's digital world. Aadhaar cards, containing sensitive information like addresses, phone numbers, and even bank account links, are prime targets for fraudsters. To address this issue, we developed a **Convolutional Neural Network (CNN) model** that **partially masks the Aadhaar's Unique Identification (UID) number**. This approach, similar to redacting bank account numbers, safeguards personal and financial data while preserving document functionality.

Our model achieves an impressive **accuracy of 94.6%** for both training and validation, effectively identifying and masking UID numbers regardless of the Aadhaar image format or orientation. This project offers a valuable tool for enhancing Aadhaar card security.

## Example

![example](Resources/abstract.png)

# Main Features

 - It does batch operations and save the final output in **.tiff** file
   format. 
  - Provide excellent PDF merging support.
  - Able to recognize UID from any type of file format such as
   jpeg, png, pdf etc. 
   - The language is different in Aadhaar in different
   regions and this is a very critical problem, but this model can recognise them easily.
   
# Algorithms Used
This model uses algorithms such as:

**1.Verhoeff Algorithm:** Aadhaar UID is a 12-digit number in which the last digit is a checksum digit
calculated using this algorithm. It utilizes some tables (multiplication, inverse and permutation) for
calculating the checksum bit. For validating, the same tables are used.

**2.ESRGANs:** Enhanced Super-Resolution Generative Adversarial Networks are capable of
generating realistic textures during single image super-resolution. It achieves better visual quality
with more realistic and natural textures than the original picture.

# Installation
**Note:** Because of some dependencies issues with Tensorflow 2.0, We have used Python 3.7.9, This project is perfectly working on Windows machines but causing some issues with Linux based systems.

**Step-1:** Clone this repo and Install Python 3.7.9 in your machine.

**Step-2:** Install **requirements.txt** by entering below command in Windows Command Prompt

    pip install -r requirements.txt

**Step-3:** Extract **poppler-0.68.0_x86** in **C:\Program Files** and provide the path of bin that is **C:\Program Files\poppler-0.68.0\bin** in the main code.

**Step-4:** Install **tesseract-ocr-w64-setup-v5.0.0-alpha.20201127** and provide its path as *pytesseract.pytesseract.tesseract_cmd =r'C:\Program Files\Tesseract-OCR\tesseract*' in code snippet.

**Step-5:** Run the code Masking.py.
