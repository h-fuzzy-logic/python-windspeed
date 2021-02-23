# Predicting windspeed of satellite images of hurricanes
This notebook was created for a Driven Data [competition](https://www.drivendata.org/competitions/72/predict-wind-speeds/).  

# Tools Used
* Google Collab Notebook w/ TPUs
* Python, Keras, Tensorflow
* Convolutional Neural Network (CNN)

# Technical Highlights
* Training set consisted of 70,000 366x366 JPG files (1 GB)
* To improve performance, Google Collab's TPUs were used  
* JPG files were convered to TFRecord format and the TFRecord files were stored in a Google Bucket
* The TFRecords were streamed in batches to the model during training 
* During training, model checkpoints (for the Best MSE) are saved to Google Drive
* At the end of training, the final model is also saved to Google Drive
