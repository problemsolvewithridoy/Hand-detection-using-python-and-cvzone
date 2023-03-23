
# Hand Detection using Python

This project is a hand detection program written in Python. It uses computer vision techniques to identify and track the location of hands in real-time using a webcam.The program will open your default webcam and display the output on the screen. It will track the location of your hand in real-time and draw a bounding box around it.

To quit the program, press the 'q' key.


let's start...............

To make this project you need to follow this step:-










## Installation

Install package with pip (for this project you need to install mentioned version module)

```bash
pip install cvzone==1.4.1
pip install mediapipe==0.8.3.1

```
    
## Deployment

To deploy this project run

```bash
#please subscribe "Problem Solve With Ridoy" youtube channel

import cv2
from cvzone.HandTrackingModule import HandDetector

cap = cv2.VideoCapture(0)
cap.set(3, 1280)
cap.set(4, 720)

detector = HandDetector(detectionCon=0.6, maxHands= 2)

while True:
  _, img = cap.read()
  hands, img = detector.findHands(img)
  cv2.imshow("Smart Camera",img)
  if cv2.waitKey(1) == ord("q"):
    break
```

# Output
![Screenshot (55)](https://user-images.githubusercontent.com/123636419/226914831-f39b653a-1bbb-49dd-93a6-e37509e6dcf3.png)




## You can follow me

Facebook:- https://www.facebook.com/problemsolvewithridoy/

Linkedin:- https://www.linkedin.com/in/ridoyhossain/

YouTube:- https://www.youtube.com/@problemsolvewithridoy

Gmail:- entridoy2@gmail.com

## If you have any confusion, please feel free to contact me. Thank you


## License
This script is released under the MIT License. Feel free to use, modify, and distribute it as you wish. If you find any bugs or have any suggestions for improvement, please submit an issue or a pull request on this repository.

