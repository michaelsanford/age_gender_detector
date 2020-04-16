# Age and Gender Classification

This code is based on the [OpenCV Age Detection with Deep Learning](https://www.pyimagesearch.com/2020/04/13/opencv-age-detection-with-deep-learning/) by [Adrian Rosebrock](https://www.pyimagesearch.com/author/adrian/), which performs automatic age detection/prediction using OpenCV, Deep Learning and Python.

It has been refined and includes gender detection as extra feature. This code only works with static images.

The code follows a simple approach:

1. Detect faces un the input image/video stream
2. Extract the ROI and apply age and gender detector algorithm to predict the age and gender of the person.

Follow Adrian's tutorial to learn more about it.

## Requirements

To properly run this example you will need to have Python installed (Anaconda distribution) and OpenCV. The code uses pre-trained Caffe models, that you can find located in the folders `face_detector`, `age_detector`, `gender_detector`.

## Usage

1. Fork the repo.
1. Clone your forked repo.
1. `pip install requirements.txt`
1. Locate a picture and run the following code:

To use pre-trained models and a confidence threshold of `0.5`, run
```
python detect.py --image [image_path]
```

You may also specify Caffe models and/or a confidence threshold:

```
python detect.py --image [image_path] --face [face_detector_path] --age [age_detector_path] --gender [gender_detector_path] --confidence [0.0 - 1.0]
```

Which will overlay results into `output.jpg` and write detections to the console.

## Other

Most of the code is extracted directly from Adrian's repository. Only the gender detection was added as extra. If you have any questions regarding this particular case, you can contact me through my [email](codingartificalintelligence@gmail.com) or [instagram](https://www.instagram.com/ai.coding/).