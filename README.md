# DETR_text_detection
This repoistory contains notebooks for training and running inference on DETR (Detection Transformers) for scene text detection. For directly running the inference code, please reach out to me for a trained model file (trained over 30 epochs on a partial ICDAR dataset which gives descent predictions). 

The main changes for adapting the original DETR for text detection are:
- ICDAR to COCO format conversion of dataset
- A single "text" category id of 0 (2 in total, one being for the background). So num_classes = 1
