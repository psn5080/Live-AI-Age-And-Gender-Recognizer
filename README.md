# Gender-and-Age-Detection

## Aim
To build a live age and gender detector that can guesstimate the gender and age of the user in a picture or through webcam.

## About the Project
In this Python Project, Deep Learning is used to accurately identify the gender and age of a person from a single image of a face. The predicted gender may be ‘Male’ or ‘Female’, and the predicted age may be one of the following ranges: (0 – 2), (4 – 6), (8 – 12), (15 – 20), (25 – 32), (38 – 43), (48 – 53), (60 – 100) (8 nodes in the final softmax layer). It is very difficult to accurately guess an exact age from a single image because of factors like makeup, lighting, obstructions, and facial expressions.

## Dataset
For this project, the Adience dataset is used, which can be found at [Kaggle](https://www.kaggle.com/ttungl/adience-benchmark-gender-and-age-classification). This dataset serves as a benchmark for face photos and includes various real-world imaging conditions like noise, lighting, pose, and appearance. The images have been collected from Flickr albums and distributed under the Creative Commons (CC) license. It has a total of 26,580 photos of 2,284 subjects in eight age ranges (as mentioned above) and is about 1GB in size. The models used have been trained on this dataset.

## Files
The `pretrained_models` folder contains the following files:
- `.pb` file: This is a protobuf file (protocol buffer) that holds the graph definition and the trained weights of the model. It is used to run the trained model.
- `.pbtxt` file: This file holds the protobuf in text format.
- `.prototxt` files: These describe the network configuration.
- `.caffemodel` files: These define the internal states of the parameters of the layers.

## Usage
### Detecting Gender and Age from an Image
Use the following command:
```sh
python [detect.py](http://_vscodecontentref_/#%7B%22uri%22%3A%7B%22%24mid%22%3A1%2C%22fsPath%22%3A%22c%3A%5C%5CUsers%5C%5Cnightfire%5C%5CDocuments%5C%5Ccode%5C%5CLive-AI-Age-And-Gender-Recognizer%5C%5Cdetect.py%22%2C%22_sep%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fnightfire%2FDocuments%2Fcode%2FLive-AI-Age-And-Gender-Recognizer%2Fdetect.py%22%2C%22scheme%22%3A%22file%22%7D%7D) --image <image_name>
```

### Note: The image should be present in the same folder where all the files are present.


Press Ctrl + C to stop the program execution.