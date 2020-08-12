# Classification
This is Machine Learning's classification method, which is a supervised learning concept which basically categorizes a set of data into classes. The most common classification problems are – speech recognition, face detection, handwriting recognition, document classification, etc.

## What I have done here
I have implemented classification of mnist dataset and hindi numbers dataset.

## Mnist Dataset Classification
###### Dataset Link
http://yann.lecun.com/exdb/mnist/
###### Model Architecture
* model = Sequential()
* Conv2D(28, kernel_size=(3,3), input_shape=input_shape)
* MaxPooling2D(pool_size=(2, 2))
* Flatten()
* Dense(128, activation=tf.nn.relu)
* Dropout(0.2)
* Dense(10,activation=tf.nn.softmax)
* optimizer='adam' 
* loss='sparse_categorical_crossentropy'
###### Model Accuracy
* loss: 0.0188
* accuracy: 0.9936 
* val_loss: 0.0450
* val_accuracy: 0.9865

## Hindi Numbers Classification
###### Dataset Link
https://www.kaggle.com/ashokpant/devanagari-character-dataset
###### Model Architecture
* model = Sequential()
* Conv2D(28, kernel_size=(3,3), input_shape=input_shape)
* MaxPooling2D(pool_size=(2, 2))
* Flatten()
* Dense(128, activation=tf.nn.relu)
* Dropout(0.2)
* Dense(10,activation=tf.nn.softmax)
* optimizer='adam' 
* loss='sparse_categorical_crossentropy'
###### Model Accuracy
* loss: 0.1301
* accuracy: 0.9615
* val_loss: 0.1194
* val_accuracy: 0.9683
