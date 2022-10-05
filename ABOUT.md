# About:

## utils

`image_preprocessing.ipynb`: 
some TACO images have an unusual orientations and not every learning library can rotate images automatically. This notebook goes through images, rotate the image to the correct orientation, deletes redundant EXIF information, and organize images.

`Unofficial_TACO_Downloader.ipynb`:
TACO dataset has an 'unofficial' version that's crowd-sourced and updated frequently. The original author's downloader fails sometimes. This notebook should be able to download the Unofficial TACO dataset stably.
Original TACO ~1500 images, Unofficial TACO ~3500 images.

## YOLOv5 based models

`yolov5x_v6.ipynb`: yolov5x v6 trained on TACO.
`yolov5x_v6_multi_GPU_DDP_mode.ipynb`: yolov5x v6 trained on TACO with multiple GPU, allowing larger batch size.
`yolov5x_v6_multi_GPU_DDP_mode_reduced_categories.ipynb`: yolov5x v6 trained on TACO with multiple GPU, and with reduced label categories. Original TACO has 60 categories of trash, while each category belongs to a "supercategory." Here, we train with 28 supercategories to reduce total number of classes.

## Detectron 2 based models

`Detectron2_Faster_RCNN.ipynb`, `Detectron2_Mask_RCNN.ipynb`, `Detectron2_RetinaNet.ipynb`: Prototypes of Faster RCNN, Mask RCNN, RetinaNet based on Detectron2.

