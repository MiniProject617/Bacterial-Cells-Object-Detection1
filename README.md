# Bacterial-Cells-Object-Detection

Identification of bacterial cells in images, under normal and acidic conditions.

## Installation

Install "tensorflow" and "tf-models-official":

```bash
!pip install -U -q "tensorflow>=2.9.2" "tf-models-official"
```

## Usage

There are 4 Google Colab Python code notebooks:

1. Augmentation_csv.ipyng

This code augments the train data by changing the images and the CSV file’s annotation coordinates.

Data needed:

- Train images (JPG)

- Annotation file (CSV)

2.  Bacteria_FasterRCNN.ipyng

This code is based on TensorFlow's notebook and model. It trains the model using the train and validation images and annotations.

This code saves the trained model for future use.

We chose to use the Faster-R-CNN model.

Data needed:

- Three folders for training, validation, and test data.

Each folder includes Images (JPG) and an annotation file (coco.json - We created those files by [RoboFlow website](https://roboflow.com/).


3. Run_Model.ipyng

This code runs images, detects the bacterial cells using the trained model, and creates an annotation file (CSV) and images with the annotations (JPG).

Data needed:

- Trained model from the previous code.
- Images (JPG)

4. Comparison_Test.ipyng (optional)

This code compares the predictions and the ground truth by printing the prediction and the ground truth annotations on the same image.

Data needed:

- annotation file (XML)

## Documentation:

We labeled the images and created all file types (CSV, XML, and coco.json) using [RoboFlow website](https://roboflow.com/)

[Trained Model](https://drive.google.com/drive/folders/1Aqk-f3SOo575UQ6ZuEfLRnLn9jucRJ2j?usp=sharing)

## Support and Feedback:

Support, bug reports, and feedback are welcome:
- Issue Tracker: [GitHub Issues](https://github.com/MiniProject617/Bacterial-Cells-Object-Detection/issues)
- Email: biomp617@gmail.com



