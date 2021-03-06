# OpenCV - LBP
Detect faces using an [OpenCV lbp cascade classifier](https://github.com/opencv/opencv/blob/master/data/lbpcascades/lbpcascade_frontalface_improved.xml).  

## Requirements
- OpenCV
- Python
- [scikit-image](https://scikit-image.org/)

## Installation
There are lots of different ways on how to install OpenCV and it's Python module.  
The easiest way would be to install it through the **unofficial** [Python package](https://pypi.org/project/opencv-python/) using Pip.  
You can also compile OpenCV on your machine yourself, there are many tutorials covering this topic already.
For OSX you can e.g. try out [this tutorial](https://www.learnopencv.com/install-opencv3-on-macos/).

### Cascade classifier
We use OpenCV's [CascadeClassifier](https://docs.opencv.org/3.4.3/d1/de5/classcv_1_1CascadeClassifier.html) class to load a
[lbp frontal face detector classifier](https://github.com/opencv/opencv/blob/master/data/lbpcascades/lbpcascade_frontalface_improved.xml).
Having said that, a big thank you to the authors Puttemans Steven, Can Ergun and Toon Goedeme.

## Running the face detection
Simply run `php index.php`, your images with face detection will be saved in `/dataset-output/opencv-lbp`.

### Note
The PHP script uses by default the `python` command line program.  
If you want to use another command line program (e.g. `python3`),
simply run `composer install` and copy the `.env.example` file to `.env` and customize the command line program.
