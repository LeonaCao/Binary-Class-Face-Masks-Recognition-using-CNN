# Binary-Class-Face-Masks-Recognition-using-CNN

This is a project completed by me and my teammates during the Deep Learning course at UConn. In this project we were applying convolutional neural network to recognize whether a human face is wearing a face mask and whether the person is wearing the mask properly.

At the beginning of the project, we gathered data by scraping images from Google Search. Since we were doing binary classification, we had two major classes, one of which is wearing face masks while the other is not. Then we created sub-categories for each class. 

In order to challenge our model and align with the reality as much as possible, we scraped images sellectively. For the Wearing Masks class, we scraped not only images with human faces wearing regular medical masks but also those wearing tricky designed masks. Whereas for the Not Wearing Masks class, we scraped images with faces either wearing nothing, scarves, hijabs, neck gaiters, masquerade masks, or even just with shaving cream or facial masks.

After dropping duplicates and those far smaller than our expectations, at last we had 2004 images in total for modeling, where there are 1203 images for training set and 801 for test set.

As our dataset is limited, we did image augmentation for our training set before modeling, extracted features from a pre-trained model VGG19, and applied fine tuning to improve our model.

Finally we got 88% validation accuracy for our model and learned that our model did not do well in recognizing tricky face masks, faces mostly covered by something other than face masks, faces wearing masks improperly, and low resolution images. So, that is where our model still need improvements.

For our images dataset, see https://drive.google.com/drive/folders/1J6dlwyh5lA1-BbbGUNPOWLzLZDY48JGQ?usp=sharing.
