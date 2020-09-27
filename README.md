# Drowsiness_Detection
***
## Note:
- Set **Eye aspect threshold** and **Yawn threshold** as per the setup of your camera for better accuracy.

#### Implementation of Drowsiness model:
###### Configuration for my model:
- EYE_AR_THRESH = 0.3
- EYE_AR_CONSEC_FRAMES = 30
- YAWN_THRESH = 6

If face is not detected by the camera, then it show a message **Distracted!! Look ahead**.
Else if eyes remain close for 30 consecutive frames, then a message is flashed **DROWSINESS ALERT!**.
If there is Yawn exceeding the threshold then message **Yawn Alert** is shown.


#### dlib’s facial landmark detector:
The dlib library is used to estimate the location of 68 (x, y)-coordinates that map to facial structures on the face.
![dlib’s facial landmark detector](https://www.pyimagesearch.com/wp-content/uploads/2017/04/facial_landmarks_68markup-768x619.jpg)


****
# Mathematical Calculations

![Mouth Aspect Ration](https://cdn-media-1.freecodecamp.org/images/QwHmcIumrY-z-gEECt3U9QtfDqHRUdYwN0N4)

![Eye Aspect Ration](https://www.pyimagesearch.com/wp-content/uploads/2017/04/blink_detection_6_landmarks.jpg)

![Eye Aspect Ration](https://www.pyimagesearch.com/wp-content/uploads/2017/04/blink_detection_equation.png)


****

## How to run the code?
- Install dlib library and other requirements.
- Execute the **yawn_and_eyeblink.ipynb** file.

## Video Description
[![Watch the video](https://i9.ytimg.com/vi/TttoLsjYp4Y/mq1.jpg?sqp=CPSNwvsF&rs=AOn4CLCEb7onO-J1iQqrri8dXS0_eYktRw)](https://youtu.be/TttoLsjYp4Y)


>>Refrence : https://www.pyimagesearch.com/2017/04/03/facial-landmarks-dlib-opencv-python/
