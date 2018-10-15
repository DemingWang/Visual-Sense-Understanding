# Object pose
## RGB methods
| Methods     |    BackBone  | Network Output|Pose Compution/refinement | Image
| ----------- | ----------- | -----------   | ----------- |----------- |
|   [RAD-2017](https://github.com/DC1991/Visual-Sense-Understanding/blob/master/Pose%20Estimation/object%20pose/Resource.md#2-rad-m--lepetit-v-2017-bb8-a-scalable-accurate-robust-to-partial-occlusion-method-for-predicting-the-3d-poses-of-challenging-objects-without-using-depth-proceedings-of-the-ieee-international-conference-on-computer-vision-2017octob-38483856-pdfread) | [VGG 16](http://www.robots.ox.ac.uk/~vgg/research/very_deep/)  | 8 corners of the projected 3D bounding box|[PnP](https://en.wikipedia.org/wiki/Perspective-n-Point) | real
|  [TEKIN-2018](https://github.com/DC1991/Visual-Sense-Understanding/blob/master/Pose%20Estimation/object%20pose/Resource.md#1-tekin-b-sinha-s-n--fua-p-real-time-seamless-single-shot-6d-object-pose-predictionpdfread)  |[YOLO V2](https://pjreddie.com/darknet/yolo/) |8 corners and 3D centroid projection |PnP| real
|  POSECNN[[XIANG-2018](https://github.com/DC1991/Visual-Sense-Understanding/blob/master/Pose%20Estimation/object%20pose/Resource.md#2018-rss-xiang-y-schmidt-t-narayanan-v--fox-d-posecnn-a-convolutional-neural-network-for-6d-object-pose-estimation-in-cluttered-scenespdfread)]|VGG 16|Semantic Labeling and Regression of 6D pose|[ICP](https://doi.org/10.1016%2F0262-8856%2892%2990066-C)(when depth is available)| real and synthetic
|SSD-6D[[KEHL-2017](https://github.com/DC1991/Visual-Sense-Understanding/blob/master/Pose%20Estimation/object%20pose/Resource.md#3-kehl-w-manhardt-f-tombari-f-ilic-s--navab-n-2017-ssd-6d-making-rgb-based-3d-detection-and-6d-pose-estimation-great-again-proceedings-of-the-ieee-international-conference-on-computer-vision-2017octob-15301538-pdfread)]|[SSD 300](https://arxiv.org/abs/1512.02325)|Viewpoint and In-plane rotation classification|Contour-based| real
|FMAP[[RAD-2018](https://github.com/DC1991/Visual-Sense-Understanding/blob/master/Pose%20Estimation/object%20pose/Resource.md#2-rad-m-oberweger-m--lepetit-v-feature-mapping-for-learning-fast-and-accurate-3d-pose-inference-from-synthetic-images-pdfread)]|VGG 16|8 corners of the projected 3D bounding box| PnP |real and synthetic

## RGB-D methods
| Methods     |    Feature Used   |Pose Compution | refinement| Learning method
| ----------- | ----------- | ----------- |----------- |----------- |
|[Branchmann-16](link)| Pixel value and depth | [Kabsch algorithm](https://doi.org/10.1107%2FS0567739478001680)| energy based| Random Forest


