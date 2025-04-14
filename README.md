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





🚗 Smart Parking Detection — Step-by-Step Process:

1. Model Initialization
The system begins by loading a pre-trained YOLOv8 object detection model, which is capable of identifying various objects such as vehicles within video frames.


2. Video Stream Handling
It opens a video file that contains footage of a parking area, which will be analyzed frame by frame to track vehicles and parking space usage.


3. Reading Object Labels
A list of object categories, such as cars, bikes, and people, is loaded from a text file. These labels are used to interpret what the detection model recognizes in each frame.


4. Parking Spot Setup
The exact positions of parking spots are predefined using a series of four points for each space, effectively marking 12 individual areas within the video’s view.


5. Frame-by-Frame Processing
The video is played one frame at a time. Each frame is resized to a consistent dimension to maintain accuracy and ensure that detections align with the parking space areas.


6. Running Object Detection
In each frame, the YOLOv8 model scans the image, detecting objects and providing their locations through bounding boxes.


7. Locating Detected Vehicles in Parking Spaces
For each detected vehicle, the program calculates its center point based on its bounding box. It then checks whether this point falls inside any of the marked parking spots using a polygonal test.

8. OCCUPANCY MARKING:  If a car is present inside a particular parking spot:
The system highlights that spot with a red boundary.
It marks the detected car with a label and a small dot at its center.
The corresponding parking slot is recorded as occupied.


11. Marking Available Spaces
If no vehicle is found inside a parking space, the system highlights that area with a green border, indicating it is available.


12. Counting Occupied and Vacant Slots
The program continuously counts how many parking spots are occupied and how many remain open, updating this data in real time as the video plays.


13. Displaying Live Status
A counter showing the current number of available parking spots is overlaid on the video display, providing real-time feedback to viewers.


14.  Visualizing the Results
The video display window shows:
Detected vehicles with their labels and markers
Parking spot outlines in red or green based on their status
Live updates of the total number of empty spaces


15. Program Termination
The system runs continuously until the user stops it by pressing a key (typically the ESC key). Once stopped, it releases the video feed and closes the display window properly.




"WHAT THIS SYSTEM ACHIEVES":



-Detects vehicles live within a parking area.

-Tracks which parking spaces are in use and which are free.

-Visually updates the status of each parking spot on the video display.

-Provides a real-time count of available parking spaces.

-Offers an efficient and clear visual monitoring system for parking management.






FEATURES:




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









