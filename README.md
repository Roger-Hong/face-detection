# face-detection
Try multiple cv models for live face detection through video camera.

The following models has been tried:

### OpenCV
OpenCV provids pretrained models for faces detection and eyes detection.

* Sample python code [here](https://docs.opencv.org/3.4/db/d28/tutorial_cascade_classifier.html)
* Pretrained model for [[face_detection](https://github.com/opencv/opencv/tree/master/data/haarcascades/haarcascade_frontalface_alt.xml)] and [[eye_detection](https://github.com/opencv/opencv/tree/master/data/haarcascades/haarcascade_eye_tree_eyeglasses.xml)]

Demo: `$ python OpenCV/face.py`

##### Test Result

* The modles can detect faces and eyes in live videos from camera on a 4 years old Mac Pro by drawing circles around face and eyes.
* The video is laggy, which is probably due to old CPU. The video should be smooth with GPU.
* The detection performs well when the face is vertical. But rotating face fails the detection.

##### Summary
OpenCV library can be used as baseline of face detection.
