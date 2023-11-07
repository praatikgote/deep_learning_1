# deep_learning_1

#(Tensorflow Test Program
Installation of Tensorflow)

import tensorflow as tf

print(tf.__version__)

print(tf.reduce_sum(tf.random.normal([1000,1000])))

#Keras Test Program

from keras import datasets

(train_images,train_labels),(test_images,test_labels)=datasets.mnist.load_data()

train_images.shape,test_images.shape


# Theano Test Program

import numpy

import theano.tensor as T

from theano import function

#Addition of two scalars
#Declaring Two Variables

x = T.dscalar('x')

y = T.dscalar('y')

#summing up the two numbers
z = x + y

f = function([x,y],z)

f(5,7)

#PyTorch Test Program Importing torch

import torch

import torch.nn as nn

print(torch.__version__)
#
