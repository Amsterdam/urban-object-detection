# Garbage detection using pytorch and YoloV3
## (Placeholder, work in progress)

[![Demo](https://img.youtube.com/vi/eP9xmQHbYCM/0.jpg)](https://www.youtube.com/watch?v=eP9xmQHbYCM)

Test and prediction code for a garbage object detection

## Predictions
To run predictions, download the cfg and weights from https://drive.google.com/open?id=1X62NUWxKD_hu9Z0ORFf25yLFkDqDAR0F

Then for example run the following the make a prediction:

```
python detector_garb.py -i samples/input5_frame281.jpg -o output --cuda
```

## Test

To run test execute the following code:

```
python test.py
```

| Class           | Images | Targets | P     | R     | mAP   | F1    |
|-----------------|--------|---------|-------|-------|-------|-------|
| all             | 115    | 579     | 0.242 | 0.941 | 0.875 | 0.376 |
| container_small | 115    | 180     | 0.38  | 0.989 | 0.979 | 0.549 |
| garbage_bag     | 115    | 223     | 0.212 | 0.964 | 0.875 | 0.348 |
| cardboard       | 115    | 176     | 0.122 | 0.869 | 0.77  | 0.231 |



## Training
For training a new model look at:

https://github.com/maartensukel/yolov3-garbage-object-detection-training

## TODO:

~~Add test, with test results to readme.~~
 Add (test) data. 
 Make readme more clear.
 Clean code. 
 Clean data from personal information. 
 Make public.