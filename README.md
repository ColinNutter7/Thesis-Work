# Thesis-Work
Code for Depth of Anaesthesia Monitoring

So, the files titled T#_CTW_FEATURES is the code for the processing and feature extraction for each of the training cases. There is an explanation in the notebook, but it's kind of incorrect. The workflow for each of these notebooks is: read in the data, perform CWT, do feature extraction on each of the wavelet coefficients, calculate moving window average for the features, write selected features to xlsx file.
All files title TEST# is the processing and feature extraction code for the test cases. They follow the same workflow as the training case notebooks.

The Anaesthesia Index file reads in the extracted training and test features. The 2 models used are: LASSO regression and a feed-forward neural network. There is a 3rd ANN in the notebook, which was redone with an additional feature, but you'll see that its commented out using comment blocks. Standard regression performance metrics are calculated for each model as well.

The signal quality index notebook uses additional patient data, with recorded BIS errors, in order to show that the new index is resistant to drops in signal quality.
