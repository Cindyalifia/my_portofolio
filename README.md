# Portofolio 
## Cindy Alifia Putri

# Detection Sentence Similarity using Word2Vec

Ketika saya melakukan intern di Vutura.io, dimana Vutura.io adalah start-up untuk platform chatbot, saya mengerjakan project untuk mengetes apakah dua buah kalimat akan similar atau tidak. Kedua kalimat dikatakan memiliki kemiripan apabila makna yang terdapat dalam dua kalimat tersebut sama. saya menggunakan cosinus similarity dari Word2Vec dengan model pretrained. Berikut adalah contoh program yang telah saya buat:

![](./images/ss1.png)

Dalam gambar tersebut terlihat bahwa kalimat pertama yang saya buat adalah ‘min, tolong dong aku pingin order baju’ sedangkan kalimat pembandingnya adalah ‘saya ingin memesan baju yang gaul min’ keduanya dinyatakan memiliki kemiripan dengan output yang dikeluarkan adalah True.


# Classification Of Shapes

**Datatrain available in test_set and training_set folder. I do predict with CNN algorithm.**

### Tools that needed to be installed are :
- Keras version 2.2.4
- matplotlib version 2.2.0

### Introduction
In this project, I make some classification to classify shapes there are circles, squares, or triangles. I use Keras library and some other library. In this project I also make some prediction after I train my program on file 'train.py', and the result to predict new image on file 'detect.py'. 

### How to run 
#### Training

```
$ python train.py
```

#### Detection
You just only need to type this on your terminal :  

```
$ python detect.py --images directory/image.png
```

### Installation 
There are something you have to do before running the program. You have to install all library we needed, if you haven't install before.

- First step, you have to install keras on your pc   
    you can watch keras installation on https://keras.io/#installation

- Second step, you have to install matplotlib on your pc   
```
$ pip install matplotlib
``` 

### Dataset
In this project, I use shapes for dataset which is circle, square, and triangle. I've got this data from https://www.kaggle.com/cactus3/basicshapes. There are 300 image containing 100 pictures each of circle, rectangle, and triangle. I split data for training set 67% and for test set 33%. 

### Result of training
After I train my program, I got the accuracy is 92.04% using 20 epoch.

![](./images/train.png)

And also I plot my training result :

![](./images/model_acc.png)

If we look closer to my image, we can see that the accuracy from my train is almost overfitting. and that's why I make 20 epochs.  
And the result for loss is :

![](./images/model_loss.png)

### Resutl of predict
I predict my model, and the result for trying to predict square image is this:

![](./images/squares_predict.png)

My program already classify square into square class. And then, when I try to predict triangle image is this:

![](./images/triangle_predict.png)

And I can say that my model to classify shapes is work. 

### My Model Result
I save my model on 'my_model.h5'.

# Crude_Oil_Prediction_Using_ANN

**I use Dataset with time series type and the output that we expected is Price od crude oil**

**Datatrain available in Europe_Oil_Price.csv**

### I do predict with ANN algorithm 

I got loss equal to 0.00005 = 0.05%

### Tools that needed to be installed are :
- Keras version 2.2.4
- Tensorflow version 1.13.0-rc2
- Pandas version 0.23.4
- Numpy version 1.16.1
- Matplotlib version 2.2.3

### Split dataset and lookback
I use 67% of dataset to data X and 33% to data Y. And also because this data is time series type, so i use lookback = 3. Lookback is how much data we use to predict one data. Of course all data still have to be fit to ann, but we have to predict with specified lookback to make data more acurate.

### I use Input layer = 64, Hidden layer = 8, Hidden layer = 8, Hidden layer = 8, Output layer = 1 and the result of crude oil predicition describe with image below 

![](./images/Result.png)

blue line is the real dataset, orange line is testX, and green line is testY


# Self_Organizing_Map

## Requirement

*  Python 3.6
*  matplotlib
*  pandas

## How to Run

Buka terminal > Pindah direktori sesuai dengan letak file > Jalankan command `python som.py` pada terminal

#### SOM

SOM adalah salah satu algoritma machine learning yang termasuk kedalam tipe Artificial Neural Network. Training algoritma SOM termasuk kedalam Unsupervised Learning.

#### Data dan Hasil

Dalam algoritma ini, akan dilakukan pemberian class atau label, atau sering disebut juga dengan clusterring. Dataset yang digunakan adalah Dataset.xls. Dalam dataset tersebut, memiliki 2 atribut yaitu x dan y, dan apabila dilakukan visualisasi data, maka akan didapatkan gambar seperti dibawah ini

![](./images/data.png)

Terlihat jelas bahwa dalam dataset memiliki 15 class yang tersebar. Apabila dilakukan proses training terhadap algoritma SOM, akan didapatkan gambar seperti dibawah ini

![](./images/result.png)

Dimana scatter kuning adalah dataset, dan scatter berwarna merah adalah hasil centroid yang didapatkan untuk menggambarkan masing-masing class dari 1 hingga 15.
