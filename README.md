# scratch_crack_detector_nn

Refer to Code Test for ML.pdf in DataSet folder for outline of the problem.

Basically, there are two types of defects in 25 areas (5 * 5 grid).  First is a red crack and second is a green scratch 
(in RGB).  

The images are 100 * 100 pixels * 3 channels (RGB).  With 2 types of defects * 25 zones = 50 classes.

One-hot encoding was used for this and the dataset size was small at 150 images so elastic transformation was used to expand 
this by four-fold to 600 images.  Elastic transformation is used on medical images that have underlying grids.  

96.7% accuracy was achieved via transfer learning on VGG-16 base model from Keras.  

