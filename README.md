# Traffic Sign Recognition

Implementation of a Convolutional Neural Network for classification using Keras.

## Usage
- Code can be accessed through the provided Jupyter Notebook file.
- ### Dependencies
- Keras
- OpenCV
- Matplotlibb
- Numpy
- Tensorflow
- Pandas
- Seaborn
- imageio

## CNN Model Details
Following is the summary of the  COnvolutional Neural Network model used for this problem:
`Model: "sequential"
**Layer (type)                 Output Shape              Param #**
conv2d (Conv2D)              (None, 60, 60, 6)         156       
max_pooling2d (MaxPooling2D) (None, 30, 30, 6)         0         
dropout (Dropout)            (None, 30, 30, 6)         0         
conv2d_1 (Conv2D)            (None, 26, 26, 16)        2416      
max_pooling2d_1 (MaxPooling2 (None, 13, 13, 16)        0         
flatten (Flatten)            (None, 2704)              0         
dense (Dense)                (None, 120)               324600    
dense_1 (Dense)              (None, 84)                10164     
dense_2 (Dense)              (None, 43)                3655
Total params: 340,991
Trainable params: 340,991
Non-trainable params: 0`


## Dataset
- GTSRB dataset is used in this project.
- Download the dataset [here](https://drive.google.com/drive/folders/1F2F7ZK62CHLIZWoOjEx-2T9OmWb96eDy?usp=sharing) and update dataset folder location in the notebook.
- Original dataset source: <http://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset>
- The dataset consists of 43 different classes of images.

### Sample Images  from Dataset
![Sample](https://github.com/asadbinkhalid/Traffic-Sign-Recognition/blob/master/Dataset%20Sample.png?raw=true)

## Citations
- J. Stallkamp, M. Schlipsing, J. Salmen, and C. Igel. _The German Traffic Sign Recognition Benchmark: A multi-class classification competition_. In Proceedings of the IEEE International Joint Conference on Neural Networks, pages 1453–1460. 2011.
