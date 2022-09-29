## Description

This code provides code to train and deploy Semantic Segmentation of LiDAR scans, using range images as intermediate representation. The training pipeline can be found in [/train](train/). We will open-source the deployment pipeline soon.

## Pre-trained Models

### [SemanticKITTI](http://semantic-kitti.org)

- [squeezeseg](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/models/squeezeseg.tar.gz)
- [squeezeseg + crf](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/models/squeezeseg-crf.tar.gz)
- [squeezesegV2](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/models/squeezesegV2.tar.gz)
- [squeezesegV2 + crf](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/models/squeezesegV2-crf.tar.gz)
- [darknet21](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/models/darknet21.tar.gz)
- [darknet53](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/models/darknet53.tar.gz)
- [darknet53-1024](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/models/darknet53-1024.tar.gz)
- [darknet53-512](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/models/darknet53-512.tar.gz)

To enable kNN post-processing, just change the boolean value to `True` in the `arch_cfg.yaml` file parameter, inside the model directory.
  
## Predictions from Models

### [SemanticKITTI](http://semantic-kitti.org)

These are the predictions for the train, validation, and test sets. The performance can be evaluated for the training and validation set, but for test set evaluation a submission to the benchmark needs to be made (labels are not public).

No post-processing:
- [squeezeseg](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/squeezeseg.tar.gz)
- [squeezeseg + crf](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/squeezeseg-crf.tar.gz)
- [squeezesegV2](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/squeezesegV2.tar.gz)
- [squeezesegV2 + crf](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/squeezesegV2-crf.tar.gz)
- [darknet21](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/darknet21.tar.gz)
- [darknet53](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/darknet53.tar.gz)
- [darknet53-1024](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/darknet53-1024.tar.gz)
- [darknet53-512](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/darknet53-512.tar.gz)

With k-NN processing:
- [squeezeseg](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/squeezeseg-knn.tar.gz)
- [squeezesegV2](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/squeezesegV2-knn.tar.gz)
- [darknet53](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/darknet53-knn.tar.gz)
- [darknet21](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/darknet21-knn.tar.gz)
- [darknet53-1024](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/darknet53-1024-knn.tar.gz)
- [darknet53-512](http://www.ipb.uni-bonn.de/html/projects/bonnetal/lidar/semantic/predictions/darknet53-512-knn.tar.gz)
