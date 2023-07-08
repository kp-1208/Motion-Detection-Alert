# Motion-Detection-Alert
This project is used to send an auto-generated email on detecting a motion in surroundings for consecutive 5 frames.

**Install the requirements by running following command in the directory:**
```bash
pip install -r requirements.txt
```
**Replace value in "src" with your Camera IP in "motion-det2.py" file.**
```python
import threading
import cv2  # pip install opencv-python
# import imutils  #pip install imutils
import time
# importing mail module
from send_mail import prepare_and_send_email

src = "YOUR CAMERA IP"
# start the webcam
cap = cv2.VideoCapture(src)
# skipping the first frame
_, _ = cap.read()
```

**Run the python file:**
```bash
python3 motion-det2.py
```

**Refer to https://github.com/kp-1208/GMail-API for creating your client_secrets.json that are used for generating emails using GMail API.**


