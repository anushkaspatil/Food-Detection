# Food-Detection using Yolov8

## Initial Steps
To kickstart the process of food detection using Yolov8, follow these initial steps:

1. **Mount the Drive in Colab Notebook**:
    Ensure you mount the drive in the Colab notebook environment to access the necessary files and directories.
2. **Install Yolov8 Model**:
    Install the Yolov8 model in the destination folder of your Google Drive where the dataset is loaded. This step is crucial for subsequent training and inference.
3. **Configure Training Parameters**:
    Within the Yolov8 model's train function, add the path of data.yaml. Customize relevant parameters such as epochs, pretrained settings, patience, etc., to align with your specific requirements.

## Dataset
Prepare and organize your dataset according to the following guidelines:

1. **Download Dataset**:
    Download the dataset in the provided format. Ensure it is accessible and stored appropriately.
2. **Upload Dataset to Google Drive**:
    Add the dataset to your Google Drive, preferably in the same folder where the Yolov8 model is installed. This ensures seamless access and integration during training.

### Structure of the dataset
Organize your dataset with the following directory structure:

```bash
 |__dataset
 |   |__images
 |   |   |__train
 |   |   |__test
 |   |   |__valid (Optional)
 |   |
 |   |__labels
 |       |__train
 |       |__test
 |       |__valid (Optional)
```

* The validation dataset is completely optional, but the train and test directories are mandatory to train the model.

* The structure consists of two main directories: 'images' and 'labels'. 
  Each directory contains subdirectories for training, testing, and optionally, validation data. 
  Ensure that your dataset adheres to this structure for seamless training with the Yolov8 model.

* Attention: While the validation dataset is optional, it's recommended for enhancing model performance. 
  However, the 'train' and 'test' directories are mandatory for successful model training.

* If the dataset provided is too large for direct download, a zip file may be provided, containing the required data. 
  Ensure that the dataset structure is maintained within the zip file for smooth processing.

By following these steps and guidelines, you'll be well-equipped to embark on your food detection journey using Yolov8. Happy coding!

## Resources
1. [Official Doucumentation Ultralytics](https://github.com/ultralytics/ultralytics)
2. [Reference Article](https://medium.com/@cascak/installing-creating-a-custom-dataset-for-yolov8-on-google-colab-a-step-by-step-guide-4ad0a725768d)
3. [Dataset](https://universe.roboflow.com/intel-n2yjd/food-detector-acbog)

## License
This project is licensed under the [MIT License](LICENSE).
