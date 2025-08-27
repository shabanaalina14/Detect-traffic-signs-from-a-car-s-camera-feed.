# Detect-traffic-signs-from-a-car-s-camera-feed.
Built an end-to-end, real-time Traffic Sign Recognition system on GTSRB (43 classes).

Trained a compact CNN with data augmentation; Adam optimizer, cross-entropy loss; achieved >95% validation accuracy (typical on GTSRB with a modest CNN; include your exact result). 
ScienceDirect

Implemented OpenCV-based candidate detection (HSV thresholding + contour filters) and live webcam inference at ~30 FPS on CPU. 
GeeksforGeeks
Stack Overflow

Shipped a desktop app (Tkinter) to demo end-to-end inference.


# Project structure
gtsrb-realtime/
├─ data/
│  ├─ Train/            # 43 class folders (0..42)
│  └─ Test/
├─ models/
│  └─ gtsrb_cnn.pth     # saved PyTorch weights
├─ src/
│  ├─ train.py          # train & eval CNN (with explicit backprop)
│  ├─ dataset.py        # GTSRB PyTorch Dataset
│  ├─ transforms.py     # augmentations
│  ├─ infer_realtime.py # OpenCV real-time detection + classification
│  └─ app_tk.py         # simple desktop app (Tkinter) wrapping the webcam demo
├─ requirements.txt
└─ README.md
