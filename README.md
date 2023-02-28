# QuickSketch
A fun and quick project to make sketches

OpenCV (Open Source Computer Vision Library) is a popular computer vision and image processing library that is widely used for real-time computer vision applications. It is a free and open-source library that was originally developed by Intel Corporation, but now it is maintained by the OpenCV community.

OpenCV provides a vast collection of functions that can be used to process and analyze images, videos, and live streams. It supports various programming languages, including C++, Python, Java, and MATLAB, and runs on different platforms, including Windows, Linux, macOS, iOS, and Android.

In Python, OpenCV can be used to perform a wide range of tasks, including image and video processing, object detection and recognition, face detection and recognition, feature extraction and matching, camera calibration, and more. It provides a simple and intuitive interface to perform complex image and video processing operations with just a few lines of code.

Import the OpenCV and NumPy modules:
Load an input image:
Convert the image to grayscale:This converts the img to grayscale using the cv2.cvtColor() function and stores the result in the variable gray_image.
Invert the grayscale image:This subtracts each pixel value in the gray_image from 255 to invert the image and stores the result in the variable inverted_image.
Blur the inverted image:This applies a Gaussian blur to inverted_image using the cv2.GaussianBlur() function with a kernel size of 21x21 and a sigma of 0. The result is stored in the variable blurred_image.
Blend the grayscale image with the blurred image using a "divide" blend mode:This blends the gray_image with the blurred_image using a "divide" blend mode to create a sketch-like effect. The resulting image is stored in the variable sketch_image.
After displaying the sketch_image, the cv2.waitKey() function waits for a key event, and the key variable stores the key code of the pressed key. If the 's' key is pressed, the cv2.imwrite() function saves the resulting sketch image as a JPEG file with the name 'sketch.jpg' and displays a message. If the 'q' key is pressed, the cv2.destroyAllWindows() function closes all windows.
