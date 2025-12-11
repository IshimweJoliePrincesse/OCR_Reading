
WHAT THIS IS
A single-file PyQt5 application that demonstrates printed-text OCR using
PyTesseract. Features:
 - GUI window (PyQt5)
 - Load image from disk
 - Live camera input (OpenCV VideoCapture)
 - Capture current camera frame into the app
 - ROI selection (click-drag on the image)
 - Run OCR on full image or ROI
 - Preprocessing (grayscale, thresholding, denoise) before OCR
 - Overlay preview (bounding boxes + recognized text) drawn on the image
 - Extracted text shown in a text area inside the GUI

DEPENDENCIES
 - Python 3.8+
 - PyQt5
 - opencv-python
 - pytesseract
 - Pillow
 - numpy

Install with pip:
    pip install pyqt5 opencv-python pytesseract pillow numpy

TESSERACT
You must have Tesseract OCR installed on your system.
 - Windows: install from https://github.com/tesseract-ocr/tesseract and set
   pytesseract.pytesseract.tesseract_cmd to the tesseract.exe path (see code comments).
 - macOS: `brew install tesseract`
 - Linux (Ubuntu/Debian): `sudo apt install tesseract-ocr`

HOW TO RUN
    python ocr_gui_pyqt5_app.py

VIDEO DEMO SUGGESTIONS (20-40s)
 - Launch app
 - Click "Load Image" and choose a printed-text photo
 - Draw an ROI around part of the image (optional)
 - Click "Run OCR" and show the extracted text in the GUI
 - Start camera, point to printed material, click "Capture Frame", run OCR

SUBMISSION
 - Put this file in a GitHub repo with this README text or include the README
   separately.
 - Record a 20-40s video demonstrating OCR working as above.


--- END README ---


