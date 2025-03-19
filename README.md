

---Color Object Detection using OpenCV and Python---

This project detects a specific color (yellow in this case) in a video stream using "OpenCV" and "PIL". 
It captures frames from a webcam, converts them to HSV color space, applies a mask to detect the color, and draws a bounding box around the detected object.  

---Features---

- Captures video from a webcam.
- Detects a specific color in real-time (yellow by default).
- Uses HSV color space for better color detection.
- Draws a bounding box around the detected object.
- Allows quitting the program by pressing the **'q'** key.


---Project Structure---

color_object_detection/
│── main.py          # Main script for object detection
│── utils.py         # Utility function to get color limits
│── requirements.txt # List of dependencies
│── README.md        # Project documentation




---requirements---
opencv-python
pillow
numpy


To install them manually, run:
pip install opencv-python pillow numpy


---How It Works---
1. Captures video frames using OpenCV.
2. Converts the frame from "BGR to HSV" color space.
3. Uses `get_limits()` from `utils.py` to determine the lower and upper HSV bounds for color detection.
4. Creates a binary mask to filter out pixels within the color range.
5. Detects the **bounding box** around the detected area and draws a green rectangle.
6. Displays the processed video feed in a window.
7. Press "q" to exit.



---Troubleshooting--

- If you get "camera index out of range", try changing:
  cap = cv2.VideoCapture(0)  # Change 0 to 1 or 2 if needed
  
- If OpenCV throws an error about "cv2.imshow", try installing OpenCV with GUI support:
  pip install opencv-python-headless


---Acknowledgments---
Special thanks to "OpenCV" and "NumPy" for making image processing easy in Python. 

--------------------
M.JAGADEESH
