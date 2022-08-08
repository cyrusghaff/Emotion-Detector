# Emotion Detector

My project sends an output to the user that says what emotion they are feeling. It can detect if the user is happy, sad, angry, surprised, fearful, neutral, or disgusted.

Image: https://user-images.githubusercontent.com/110626228/183310632-98b22769-f099-4d90-bce2-f9eca59b6eb5.png

# The Process

I trained my model using a dataset that I found online. It cointainted the seven basic emotions that I used as the classes for my model. After training my model for an hour all of the images were in their files. However I had to code something to move the file to each of the emotions. After doing so, my project was finally ready to run. I uploaded an image and it told me what percent of everything the person was by using the imagenet network.

## Running this project

1. Make sure that you are in visual studio code and are inside the nano.
2. Cd into jetson-inference/python/training/classification.
3. Create a folder called data.
4. Extract the 
5. Add the models folder from GitHub.
6. Go back into the classification directory
7. Type: NET = models/emotions
8. Type: DATASET = data/emotions
9. Type: 

[View a video explanation here](video link)
