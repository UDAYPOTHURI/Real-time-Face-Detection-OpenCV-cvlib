# Real-time-Face-Detection-OpenCV-cvlib

This project uses OpenCV and cvlib to perform real-time face detection on a video stream from a webcam.

## Installation

To use this project, you'll need to have OpenCV and cvlib installed. You can install them using pip:

pip install opencv-python

pip install cvlib

You'll also need to download the `Real-time-Face-Detection-OpenCV-cvlib.ipynb` file from the GitHub repository. You can do this by clicking on the "Code" button on the repository page and selecting "Download ZIP". Once you've downloaded and unzipped the file, you can open it in a Jupyter notebook.

## Usage

To use this project, simply run the `Real-time-Face-Detection-OpenCV-cvlib.ipynb` file in a Jupyter notebook. The code will access your webcam and display a video stream with faces detected in real-time.

Here's a detailed explanation of how the code works:

1. The code starts by importing the necessary libraries: `cv2` and `cvlib`.
2. It then accesses the webcam using `cv2.VideoCapture()`.
3. A while loop is entered that runs until the user presses the "q" key.
4. Inside the loop, a frame is read from the webcam using `.read()`.
5. Faces are detected in the frame using `cvlib.detect_face()`.
6. If any faces are detected, their coordinates are obtained from the returned list.
7. A for loop is entered that iterates over each detected face.
8. Inside the for loop, a rectangle is drawn around each face using `cv2.rectangle()`.
9. The confidence score for each face is displayed on the frame using `cv2.putText()`.
10. The frame is displayed using `cv2.imshow()`.
11. The code waits for 1 millisecond for a key press using `cv2.waitKey()`. If the "q" key is pressed, the while loop is exited.
12. After exiting the while loop, the webcam is released using `.release()` and all windows are destroyed using `cv2.destroyAllWindows()`.
