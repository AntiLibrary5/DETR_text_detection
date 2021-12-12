# DETR for scene text detection
This repoistory contains notebooks for training and running inference on DETR (Detection Transformers) for scene text detection. For directly running the inference code, please reach out to me for a trained model file (trained over 30 epochs on a partial ICDAR dataset which gives descent predictions). A huge thanks to NielsRogge implementation from which most of the DETR code is adapted from.

The main changes for adapting the DETR for text detection are:
- Text detection datasets are typically in ICDAR format which need to be converted to COCO format
- A single "text" category id of 0 (2 in total, one being for the background). So num_classes = 1

This work can also be interesting to people wanting to train DETR on their own custom dataset.

