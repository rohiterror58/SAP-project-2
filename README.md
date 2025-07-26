# Face Detection System with WhatsApp Integration

This project is a real-time face detection system using OpenCV. It detects faces in the camera feed, draws rectangles around them, and triggers actions like saving the detected faces as images and sending them via WhatsApp using `pywhatkit`.

## Features

- **Real-time Face Detection:** Detects and draws rectangles around faces.
- **Line Crossing Detection:** Triggers a warning and saves an image when a face crosses a predefined line.
- **WhatsApp Integration:** Automatically sends detected face images via WhatsApp.
- **Image Management:** Optionally deletes saved images after sending.

## Installation

1. **Clone the Repository:**
    ```sh
    git clone https://github.com/yourusername/facedetection-whatsapp.git
    cd facedetection-whatsapp
    ```

2. **Install Dependencies:**
    ```sh
    pip install opencv-python numpy pywhatkit
    ```

3. **Download Face Detection Cascade:**
    Download the `haarcascade_frontalface_default.xml` file from the OpenCV GitHub repository and place it in the specified directory (`D:/downloads/SpyEye-main/SpyEye-main/XML_Files/`).

## Configuration

Update the constants in the script as needed:

- `LINE_Y`: The y-coordinate of the line for line-crossing detection.
- `WHATSAPP`: Set to `True` to enable WhatsApp integration.
- `DELETE_SAVED_IMAGES`: Set to `True` to delete saved images after sending.
- `TIME_INTERVAL`: Interval between image saves when faces cross the line.
- `WHATSAPP_NUMBER`: The WhatsApp number to send images to.
- `IMAGE_SEND_DELAY`: Delay between sending consecutive images via WhatsApp.

## Usage

Run the main script to start the face detection system:

```sh
python facedetection.py
