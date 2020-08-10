# Object Detection using OpenCV

Pranshu Varshney 10th Aug 2020

### Object Detection code using YOLO. The repository contains:

1. yolo.py and yolo_video.py - Python code to run YOLO model to produce object detection output in image and video respectovely.
2. images: Contains images to be tested
3. output: Contains the output for both image and videos
4. videos: Contains videos to be tested. Folder is empty add your videos to test
5. yolo-coco: Contains YOLO models weights and configuration used for prediction.Add yolo weights in this folder from [Yolo weights](https://pjreddie.com/media/files/yolov3.weights)

## Object Detection in Image

To run object detection in image run the below command:

```
python yolo.py --image images/dining.jpg --yolo yolo-coco
```

Note: The commands take dining image from image folder as input. YOLO model config files from yolo folder

## Object Detection in Video

To run object detection in video run the below command:

```
python yolo_video.py --input videos/traffic.mov --output output/traffic.mov --yolo yolo-coco
```

Note: The commands take traffic video from video folder as input and the output video is saved in the output folder with name traffic.mov with csv file contianing what object was detected.

Ref:https://www.pyimagesearch.com/2018/11/12/yolo-object-detection-with-opencv/
