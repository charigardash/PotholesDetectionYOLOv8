# Image Segmentation & Pothole Detection

# Google Colab File Link (A Single Click Solution)

The google colab file link for yolov8 segmentation and tracking is provided below, you can check the implementation in Google Colab, and its a single click implementation ,you just need to select the Run Time as GPU, and click on Run All.

[Google Colab File](https://colab.research.google.com/drive/1MJwthnlppm0h0nfO5ScwHBq3c_lnrg1h#scrollTo=2I8v9DamvxmB)

# Tech stack
![python](https://camo.githubusercontent.com/0562f16a4ae7e35dae6087bf8b7805fb7e664a9e7e20ae6d163d94e56b94f32d/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f707974686f6e2d3336373041303f7374796c653d666f722d7468652d6261646765266c6f676f3d707974686f6e266c6f676f436f6c6f723d666664643534)

# Object Segmentation and Tracking (ID + Trails) using YOLOv8 on Custom Data

## Clone the repository

```git clone https://github.com/charigardash/PotholesDetectionYOLOv8.git```


## Downloading the Potholes on a Road Video from the Google Drive
[Potholes on Road Video](https://drive.google.com/file/d/1MxNWhRhbAxFjY6S0iz8UsqYNZhiVePH_/view?usp=sharing)

## My roboflow workspace containing the pothole dataset
[Roboflow Workspace](https://app.roboflow.com/mdosamaansari/potholedetectionyolov8-jsbn7/browse?queryText=&pageSize=50&startingIndex=0&browseQuery=true)

Run the code with mentioned command below.

+ For training the data
  
  ```
  !yolo task=detect mode=train model=yolov8m.pt data={dataset.location}/data.yaml epochs={number of epochs} imgsz=640
   ```
+ For yolov8 segmentation + Tracking & prediction
  
  ```
  !yolo task=detect mode=predict model={HOME}/runs/detect/train/weights/best.pt conf=0.25 source='/content/drive/MyDrive/demo.mp4'
  ```

