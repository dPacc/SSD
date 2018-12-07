# Deep Learning based Object Detection with OpenCV

We use MobileNets to predict the classes. We call these networks “MobileNets” because they are designed for resource constrained devices such as your smartphone. MobileNets differ from traditional CNNs through the usage of depthwise separable convolution.

The MobileNet SSD was first trained on the COCO dataset (Common Objects in Context) and was then fine-tuned on PASCAL VOC reaching 72.7% mAP (mean average precision).

We used the MobileNet SSD + deep neural network ( dnn ) module in OpenCV to build our object detector.


### Usage: -

We parse our command line arguments with the following:

* image : The path to the input image.
* prototxt : The path to the Caffe prototxt file.
* model : The path to the pre-trained model.
* confidence : The minimum probability threshold to filter weak detections. The default is 20%.

#### Run
 
```
$ python deep_learning_object_detection.py \
	--prototxt MobileNetSSD_deploy.prototxt.txt \
	--model MobileNetSSD_deploy.caffemodel --image images/example_01.jpg
```

Alternaltely, you can add custom images onto the /images folder and test.

