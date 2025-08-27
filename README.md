# Detect-traffic-signs-from-a-car-s-camera-feed.
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
