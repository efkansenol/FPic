# FPic
A image file extension I created myself

# How to use
## How to convert a image file to .fpic
Open your image file with FPic.exe and click the Convert button. You can then edit the path and name of your .fpic file in the window that opens. After clicking Save, your .fpic version of the file will be created!

![FPİC](https://github.com/user-attachments/assets/aacf7de9-6e4d-4604-bca2-28acfb257701)

## How to open a .fpic file
You can view your file by opening the .fpic file with FPic.exe. FPic.exe will perform the operations according to the type of file opened.

![0808(1)](https://github.com/user-attachments/assets/542e0b44-8b69-4a50-850b-c0c91a6f9bda)



# How it works
## When a file is converted to a .fpic file:
First, when a file is converted to a .fpic file, it is read as a bitmap, and the RGB (JPEG) or RGBA (PNG) data inside is retrieved. Then, a new .fpic file is created with an FKNP tag inside. This tag enables the file to be identified as a .fpic file when opened. Next, the file size data is written into the file. Then, the initial Bitmap data is written into the file. Finally, the file is compressed using the Brotli library to create the .fpic file.
## When opening a .fpic file
When the file is opened, the FKNP tag written at the beginning is checked first. Once the file is confirmed to be .fpic, the size data inside is read and processed into the Form. Then, the remaining Bitmap data is read and transferred to the Pic
