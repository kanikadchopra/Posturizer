# Posturizer
Hack the North 2019 Project; we created a web app that would detect if you had bad posture and a voice feature to tell you how to fix your posture. This code is for the preprocessing of the training images we used on our Microsoft Azure AI Custom Vision model to recognize posture classes.


The link to the devpost associated with this project is here:

## What We Did
We collected images of people slouching forward, leaning back and leaning left and right for bad postures and with a straight back for good postures. This gave us 5 classes to use for our single class classification. The Jupyter Notebook shows how we considered first using edges to augment the photos and remove facial features so that they wouldn't distract the model and for privacy issues. The second method is the one we used - we used OpenCV to detect faces in the training photo dataset and then blurred out the faces so that the model focused on the posture and did not associate certain faces with certain postures and as well to preserve the privacy of the volunteers featured. 

## Parts not Included
After our Microsoft Azure AI Custom Vision model was trained on this data, we tested it using our training set. The images are not included for privacy preservation and as well the front end is not included as other team members have placed them in a private repository. The parts included mainly show the preprocessing using OpenCV before the image classification began. 
