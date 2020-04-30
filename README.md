# Emotion Detection
Detecting the emotion of human with the help of computer vision to distinguish between 5 types of emotion (anger, happy, sad, surprise, unknown).
Used an convolutional neural network model (CNN) inspired from VGG-16 model architecture.

The model has been trained on fer2013 dataset and got 60 percent in [Google Colabaratory's](https://colab.research.google.com/) GPU so it may not
be accurate but performs well. you are welcome to train it more.

## Built using
```
Python-3
Tensorflow
Opencv
```

## Setting up in your local machine
We can set this project in your local machine to start predicting.

#### Step - 1
Open a `terminal`, clone the `Question-analyzer` repository and go into the directory using the command `cd`.
```bash
git clone https://github.com/sherwin7/Emotion_Detection.git

cd Emotion_Detection
```

#### Step-2
Check `python-3` is installed then install `pip` manager for python-3 and install `virtual environment`.
```bash
#Checking python is installed
python3 --version 

#Installing pip manager
sudo apt install python3-pip

#Checking pip is installed for python3
pip3 --version

#Installing virtual environment
sudo pip3 install virtualenv
```

#### Step-3
Setting up `virtual environment`.
```bash
#Creating virtual environment
virtualenv -p python3 venv

#Activating the virtual environment venv
source venv/bin/activate
```

#### Step-4
Now we have to install all the dependencies using pip in our virtual environment from `requirements.txt`.
Check `requirements.txt` to know what are all the dependencies used.
```python
pip install -r requirements.txt
```

#### Step - 5
We can run the `emotion_detection.py`. Here the video used are in `test_videos` you can keep yours and try or if you want to use a 
live video from your webcam In 'emotion_detection.py` change the line `31` (i.e) `cap = cv2.VideoCapture('./test_videos/test3.mp4')`
to `cap = cv2.VideoCapture('0')` which takes the default camera input and press `q` to quit from the program.
```
python emotion_detection.py
```

## Result
