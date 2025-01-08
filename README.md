# ObjectDetection-v1
[![Python](https://img.shields.io/badge/Python-3776AB.svg?logo=python&logoColor=white)](https://www.python.org/) 
[![Ultralytics](https://img.shields.io/badge/Ultralytics-00875A.svg?logo=ultralytics&logoColor=white)](https://github.com/ultralytics) 
[![YOLO](https://img.shields.io/badge/YOLO-FF69B4.svg?logo=yolo&logoColor=white)](https://github.com/ultralytics/yolov5)
![Artificial Intelligence (AI)](https://img.shields.io/badge/Artificial%20Intelligence%20(AI)-orange.svg?logo=ai&logoColor=white)
![Object Detection](https://img.shields.io/badge/Object%20Detection-EE4C2C.svg?logo=object-detection&logoColor=white)
![Last Updated](https://img.shields.io/badge/Last%20Updated-June%202023-green.svg)

### Backup of Old Project (June 2023)

This is a backup of an old project that was focused on object detection. The project was based on the following tutorials:

- [Murtaza's Workshop - Robotics and AI's Object Detection Tutorial](https://www.youtube.com/watch?v=WgPbbWmnXJ8&ab_channel=Murtaza%27sWorkshop-RoboticsandAI)
- [Computer Vision Zone's Object Detection Course](https://www.computervision.zone/courses/object-detection-course/)

The project was written in Python and uses the YOLOv8 object detection model.

### About the Project

Section 3.2: Applying YOLOv8 on static image given by path specified in the "Parameters" section.

![alt text](/docs/image.png)

Section 3.4: Applying YOLOv8 on video given by path specified in the "Parameters" section.

![alt text](/docs/vid1.gif)

Section 3.5.1: Instance identification with Abrewlay Sort library (from tutorial) for tracking objects.

![alt text](/docs/vid2.gif)

Section 3.5.2: Instance identification with custom-implemented algorithm for tracking objects.

![alt text](/docs/vid3.gif)

- More resistent to lost frames compared to the Abrewlay Sort library.
- Can accumulate labels from previous frames.

Section 3.6: Car Counter (for counting cars and people)

![alt text](/docs/vid4.gif)

- Simple algorithm for counting cars across the line by masking the image before detection.
- Utilized the algorithm in sectino 3.5.2 for tracking objects to ensure that a car is not detected twice.

### Execution

Start a new virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate # linux or windows WSL
.\venv\Scripts\activate # windows cmd
```
Then install the requirements:
```bash
pip install -r requirements.txt
```
Finally, run the jupyter notebook `Object Detection.ipynb` within the virtual environment.
