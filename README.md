# Smart-Parking-Surveillance-AI-Model
This is my submission for the **Smart Parking &amp; Surveillance AI Model Challenge**. The project detects cars in a parking lot using **YOLOv8** and **OpenCV**, counts the number of occupied and empty parking spaces


The system detects vehicles in a video using **YOLOv8**.
12 predefined parking areas are mapped using polygon points.
The center of each detected car is checked against the parking areas.
Occupied parking areas are highlighted in **red**, empty ones in **green**.
The number of available (empty) spots is displayed in real-time on the video.






  HOW TO RUN:


  
Download YOLOv8 pre-trained weights (yolov8s.pt) and place them in the models/ directory.
Place your video file (parking1.mp4) inside the videos/ folder.
Make sure coco.txt is present in the root directory (with COCO class labels).
Run the script:
python testcount.py




✅ FEATURES:




Real-time vehicle detection,
Parking space occupancy counting,
Dynamic visualization of occupied and empty slots,
Occupied spots shown in red, empty in green,
Free spot count displayed live,
YOLO-based action detection (like 'falling down'),
Using pose estimation or action recognition datasets,
Real-time alerts on abnormal activity.



CONTACT INFO:


Name: KARANAM SARVAN

Email: karanamsarvan@gmail.com

CONTACT NUMBER: 6303306015









