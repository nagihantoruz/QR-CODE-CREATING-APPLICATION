###  QR Code creating Application 

This project takes a URL entered by the user and generates a QR code, saving it as an `.svg` file.

#### Usage

1. Run the program.
2. Enter the desired URL (e.g., `https://openai.com`).
3. The QR code will be saved as **qrcode.svg**.

#### Code Explanation

```python
import pyqrcode

# Get URL input from the user
url = input("enter url to generate qr code: ")

# Create a QR code object
qr_code = pyqrcode.create(url)

# Save the QR code as an SVG file
qr_code.svg('qrcode.svg', scale=5)
```

* **pyqrcode.create(url):** Generates a QR code from the given text or URL.
* **.svg():** Saves the QR code as an `.svg` file. The parameter `scale=5` controls the size of the output.

#### Example Output

You can open the QR code in a browser or scan it with your phone’s camera.

