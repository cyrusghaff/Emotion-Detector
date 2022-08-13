# Emotion Detector

My project sends an output to the user that says what emotion they are feeling. It can detect if the user is happy, sad, angry, surprised, fearful, neutral, or disgusted.

Image: https://user-images.githubusercontent.com/110626228/183310632-98b22769-f099-4d90-bce2-f9eca59b6eb5.png

# The Process

I trained my model using a dataset that I found online. It cointainted the seven basic emotions that I used as the classes for my model. After training my model for an hour all of the images were in their files. However I had to code something to move the file to each of the emotions. After doing so, my project was finally ready to run. I uploaded an image and it told me what percent of everything the person was by using the imagenet network.

## Running this project

1. Download and setup the Nvidia Jetson-Inference Project linked [here](https://github.com/dusty-nv/jetson-inference) 
2. Make sure that you are in [Visual Studio Code](https://code.visualstudio.com/) and are connected to the nano via ssh
3. Cd into jetson-inference/python/training/classification
4. Clone this repository
5. Setup an environment variable NET = Emotion-Detector/emotions_model
6. Setup an environment variable DATASET = Emotion-Detector/emotions_training_data
7. Run the jetson-inference imagenet.py using the command below:
```
imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt input_image output_image
``` 
8. Substitue input_image and output_image in reference to the input image and output image you want to proccess
[View a video explanation here](video link)
