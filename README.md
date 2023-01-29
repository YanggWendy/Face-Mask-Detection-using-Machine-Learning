# Face-Mask-Detection-using-Machine-Learning
## Dataset
We use the given Face mask dataset on Kaggle. This dataset contains 853 images belonging to the 3 classes, as well as their bounding boxes in the PASCAL VOC format. The classes are: 1) With mask; 2) Without mask; 3) Mask worn incorrectly.
To do the classification task, we clip the face images from the original dataset using given annotation boxes and we finally got clipped 4072 images with three classes: 1) With mask; 2) Without mask; 3) Mask worn incorrectly

## Task
The main machine learning task we performed on this dataset is to detect mask, no mask and incorrectly worn masks.
To be specific, we take images as inputs, and output the bounding boxes together with the classes they belong to. The three classes are 1) with mask; 2) without mask; 3) mask worn incorrectly. We mainly use F score as the performance metrics, and mAP(@0.5,@.5:.95) as the auxiliary metrics.

Here TP is the number of correct objects given, FP is the number of incorrect objects given, FN is the number of missed objects. Correct objects means 1) predicted bounding box has IoU > 0.5 with ground truth; 2) predicted class of the object is the same as the true class.

We approach this task through two different paths, [Face Detection + Classification](https://github.com/YanggWendy/Face-Mask-Detection-using-Machine-Learning/tree/main/Retinaface%2Bclassification) and [YOLOv5 object detection model](https://github.com/YanggWendy/Face-Mask-Detection-using-Machine-Learning/tree/main/YOLOv5).

For more information, please refer to report: https://github.com/YanggWendy/Face-Mask-Detection-using-Machine-Learning/blob/main/Face%20Mask%20Detection%20using%20Machine%20Learning.pdf
