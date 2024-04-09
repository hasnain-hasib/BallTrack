# Ball Tracking using Color Detection

This Python script demonstrates real-time object tracking using color detection. It captures video from the webcam or a video file, detects objects of a specific color range, and tracks their movement by drawing trails on the video frame.

## Prerequisites

Before running the script, ensure you have the following dependencies installed:

- Python 3.x
- OpenCV (`pip install opencv-python`)
- NumPy (`pip install numpy`)
- imutils (`pip install imutils`)

## Usage

1. Clone the repository or download the script.
2. Ensure your webcam is connected and accessible, or provide a path to a video file using the `-v` argument.
3. Run the script using the command `python object_tracking_color_detection.py`.
4. Perform object tracking by moving an object of the specified color range in front of the camera.
5. Press 'q' to exit the script.

## Script Overview

- The script uses OpenCV for video capture, color detection, contour finding, and drawing on the video frame.
- It utilizes a deque to store the tracked object's centroid coordinates and draw trails.
- The script continuously captures video frames, preprocesses them by resizing and blurring, and converts them to the HSV color space.
- It applies a mask to detect objects within the specified color range and performs erosion and dilation to remove noise.
- Contours of the detected objects are found and used to determine their centroids.
- Trails are drawn on the video frame to track the movement of the detected objects.
- Pressing 'q' during execution quits the script.

## Acknowledgments

- This script uses OpenCV for computer vision tasks and NumPy for numerical computations.
- Special thanks to the imutils library for providing convenient functions for image processing.

## References

- [OpenCV](https://opencv.org/)
- [NumPy](https://numpy.org/)
- [imutils](https://github.com/jrosebr1/imutils)

Feel free to modify and extend this script according to your requirements! If you have any questions or suggestions, please feel free to reach out.
