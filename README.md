# yolov8_optical_character_recognition
 yolov8 trained for extracting text, label, and bounding boxes around texts in image


I trained yolov8 model for 10 epochs on the open_poetry dataset of around 4000 images in Validation, training, and testing from the Roboflow repository. The model used by me is the yolov8 type n model from Ultralytics and i trained the base model to become a model that's adept at capturing text segments on images of different fonts and colors. The input is a 640 by 640 image, and the output is a list of 1) labels for the style of the text 2) bounding box coordinates of the text and 3) confidence level of detection.

I trained the model for 10 epochs only on a RTX 2070 cause it takes too long otherwise but the results are great. The model is able to bound the boxes perfectly however the labels are sometimes incorrect. Some texts are also not picked up but probably will if u train it for longer. I used CUDA for acceleration and the process took 10 minutes. Also tried with RT-DETR but the architecture is too big to train for me.

Consult Dataset for some testing data for normal bounding boxes on the COCO dataset and consult the Poetry-Vision-1 dataset for the training and testing datasets. Within the ../Run/Detect directory, train16 contains the model weights that are trained and can be used. its called best.pt under /weights.