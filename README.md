# yolov5_to_cpp_opencv_deploy

record my experience of deploy yolov5 to opencv in cpp plantform.

methord:
1. git clone https://github.com/ultralytics/yolov5/tree/v3.1    (yolov5 v3.1  ,some code changed with edition)
2. cd ./yolov5
3. pip install -r requirements.txt
4. pip install coremltools>=4.1 onnx>=1.9.0 scikit-learn==0.19.2 
5. python models/export.py --weights yolov5s.pt --img 640 --batch 1    # export at 640x640 with batch size 1

6. using code myyolo.cpp yolo.h in this repo. (I used opencv 3.4.14 , c++11)
7. adding img and xxx.onnx into cpp proj, change imgpath and .onnx path parameters.
8. run.


.vscode is my vscode config file, just for reference.
