# Classifying Monkey Species using (Xception as the base) Model. 
Some code for a pretrained CNN models to classify 10 monkey species, as found on Kaggle 

The link to that data and project is https://www.kaggle.com/slothkong/10-monkey-species 

In addition to the data provided for training and validation, I used googliser.sh,
a bash script, for downloading images from google images, which I then used to create 
my own data for testing. As this is a rough around the edges project, I cleaned up 
this new data--which consisted of around 100 new images in the each of the 10 categories--
by taking out things like maps, that obviously were not monkeys themselves.
I left the rest of it to Keras' data generator and image preprocessing features. 

The base model is Xception using the imagenet pretrained model weights. 

In practice, I found using SGD was better than using adam optimizer. 
Trained on 5 epochs to get a good sense of how things were going. 
More exploration of hyperparameter tuning is needed. 

