# Density-map-by-Yolo-v7-Model
Ther are three versions of the yolo v7 
## Version -1 
Object detection in a single frame 

Directly execute Copy of Training YOLOv7 on Custom Data.ipyb

## Version-2
Object detection in a video

Add your trained weights yolov7 object detection weights (Best.pt) and add detect_and_blur.py file 

Run the code with mentioned command below.
#if you want to change source file
!python /content/yolov7-object-blurring/detect_and_blur.py --weights /content/best.pt --source "/content/left20024_07_07_22_12_00_Uhr_wbmode1.mp4" --conf 0.3

Output file will be created in the working-dir/runs/detect/ with original filename

## Version -3
Object Tracking in a video



Add your trained weights yolov7 object detection weights (Best.pt) and add detect_and_track.py file 

Run the code with mentioned command below.
#if you want to change source file
python detect_and_track.py --weights yolov7.pt --source "your video.mp4"

#for specific class (person)
python detect_and_track.py --weights yolov7.pt --source "your video.mp4" --classes 0

Output file will be created in the working-dir/runs/detect/obj-tracking with original filename

Reference:
https://github.com/RizwanMunawar/yolov7-object-tracking/blob/main/README.md
