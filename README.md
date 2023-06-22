# Yellow Pixel Extraction and Tracking

This Python code allows you to detect and track yellow pixels in an image or video. It utilizes the OpenCV library for image processing and computer vision tasks.

## Prerequisites

Make sure you have the following dependencies installed:

- Python 3.x
- OpenCV (cv2)

You can install OpenCV using pip:

```shell
pip install opencv-python
```

Usage
- Clone the repository or download the code files.
- Place the image or video file you want to process in the same directory as the code files.
  
For image processing:
- Open the yellow_pixel_detection.py file.
- Modify the image_path variable to the path of your input image file.
  
Run the script:
```shell
python yellow_pixel_detection.py
```

- The output will be displayed, showing the yellow pixels detected in the image.
For video processing:
- Open the yellow_pixel_tracking.py file.
- Modify the video_path variable to the path of your input video file.
Run the script:
```shell
python yellow_pixel_tracking.py
```

- The video will be played, and the yellow pixels will be tracked in real-time.
## Algorithm
The code uses the following algorithm for yellow pixel detection:

- Convert the image/video frame from BGR color space to HSV color space.
- Define a lower and upper range for yellow color in HSV.
- Threshold the HSV image to obtain a binary mask of yellow pixels.
- Apply morphological operations (e.g., erosion and dilation) to remove noise and improve the mask.
- Find contours of the yellow regions in the mask.
- Draw bounding rectangles around the detected yellow regions.

## Customization
You can customize the code according to your requirements. Here are some suggestions:

- Adjust the lower and upper range of yellow color in the HSV space (lower_yellow and upper_yellow variables) to fine-tune the detection.
- Modify the morphological operations (e.g., kernel size, iterations) in the preprocess_mask function to improve noise removal.
- Experiment with different methods for tracking the yellow pixels, such as centroid tracking or Kalman filtering.

## Contact
If you have any questions, feel free to contact me at [udaysankar2003@gmail.com].
