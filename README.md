# Cat-Vs-Dog-Deployed-Tensorflow-using-serving
-------

In this project I built a Cat-Dog classifier with Tensorflow using MobilenetV2 architecture.
The web app built in Python was hosted on my local host. 
The app has an option to upload an image from local disk and submit. The image was jsonified and sent to the model and result rendered back on the predictions page.
The web app was hosted on a dockerized version of the instance using Tensorflow serving.

## Below are the main components inplace:

## 1. The Flask App
###  Created functional web app with Flask.
## 2. Index Template
### Added a template for the index page. And a base template which extends a Bootstrap base template.
## 3. TensorFlow Serving
### Created a docker instance with TensorFlow Serving image.
We will deploy and serve our binary classifier model in the docker instance.
## 4. Getting Predictions
### Created a module which sends post request to the model server with input image tensor.The module will also post process the predictions obtained from the model server.
## 5. Connecting the Model Server to the App
### Created a functionality in order to be able to upload an image file.
## 6. Displaying the Results in the App
### Finally, Created a show.html template, where I displayed the uploaded image along with its predicted class
