# Gender-and-Age-Detection-

<h3>Introduction:</h3><hr>
Gender and Age Detection is one of the interesting python project which detects human's age and gender through an image and webcam using OpenCV and CNN.

<h3>Objective:</h3><hr>

To build a gender and age detection that can approximately guess the gender and age of the person (face) in a picture or through webcam.

<h3>About the Project:</h3><hr>

In this Python Project, I had used Deep Learning to accurately identify the gender and age of a person from a single image of a face. I used the models trained by Tal Hassner and Gil Levi. The predicted gender may be one of ‘Male’ and ‘Female’, and the predicted age may be one of the following ranges- (0 – 2), (4 – 6), (8 – 12), (15 – 20), (25 – 32), (38 – 43), (48 – 53), (60 – 100) (8 nodes in the final softmax layer). It is very difficult to accurately guess an exact age from a single image because of factors like makeup, lighting, obstructions, and facial expressions. And so, I made this a classification problem instead of making it one of regression.

<h3>Dataset:</h3><hr>

For this python project, I had used the Adience dataset; the dataset is available in the public domain and you can find it <a href = "https://www.kaggle.com/datasets/ttungl/adience-benchmark-gender-and-age-classification">here</a>. This dataset serves as a benchmark for face photos and is inclusive of various real-world imaging conditions like noise, lighting, pose, and appearance. The images have been collected from Flickr albums and distributed under the Creative Commons (CC) license. It has a total of 26,580 photos of 2,284 subjects in eight age ranges (as mentioned above) and is about 1GB in size. The models I used had been trained on this dataset.

<h3>Technology Used:</h3><hr>

<li><p>Programming Language : Python </p></li>
<li><p>Version : Python 3.10 </p></li>
<li><p>Tools Used :  OpenCV and argparse </p></li>
<li><p>Operating System : Windows </p></li>


<h3>Python Libraries Required:<h3><hr>

<ul>
<li>OpenCV</li>
<h5>pip install opencv-python</h5>
</ul>

<ul>
<li>argparse</li>
<h5>pip install argparse</h5>
</ul>

<h3>Project Contents:<h3><hr>

<h6>opencv_face_detector.pbtxt</h6>
<h6>opencv_face_detector_uint8.pb</h6>
<h6>age_deploy.prototxt</h6>
<h6>age_net.caffemodel</h6>
<h6>gender_deploy.prototxt</h6>
<h6>gender_net.caffemodel</h6>
<h6>a few pictures to try the project on</h6>
<h6>gad.py</h6>

For face detection, we have a .pb file- this is a protobuf file (protocol buffer); it holds the graph definition and the trained weights of the model. We can use this to run the trained model. And while a .pb file holds the protobuf in binary format, one with the .pbtxt extension holds it in text format. These are TensorFlow files. For age and gender, the .prototxt files describe the network configuration and the .caffemodel file defines the internal states of the parameters of the layers

<h3>Usage:</h3><hr>

<p><li>Download my repository</li></p>
<p><li>Open your Command Prompt or Terminal and change directory to the folder where all the files are present.</li></p>
<p><li>Detecting Gender and Age of face in an image use command</li></p>
<ul>
<h5><b>python gad.py --image <image-name></b></h5>
</ul>

Note: The image should be present in the same folder where all the files are present

<p><li>Detecting Gender and Age of face through webcam use command:</li></p>
<ul>
<h5><b>python gad.py</b></h5>
</ul>
<p><li>Press Ctrl-C to stop the program execution</li></p>

<h3>Working:</h3><hr>


![myphoto](https://github.com/Praveen-ASE/Gender-and-Age-Detection-/assets/148997369/e9048a0a-a9bd-4ec8-af6b-1b8f48f5d611)




![Screenshot (35)](https://github.com/Praveen-ASE/Gender-and-Age-Detection-/assets/148997369/d49558fe-1d26-4478-909f-560c730c9435)


<h3>Conclusion:</h3><hr>

The age and gender detection using OpenCV will be very beneficial in authorization purposes, medical purposes or surveillance purposes. The CNN and OpenCV combined can give great results. The OIU-Adience dataset used in the project gives result with greater accuracy. We used protocol buffer and  caffee  model files. This project shows how OpenCV can be used for face detection without any other complicated process.



