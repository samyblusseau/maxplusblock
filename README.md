# maxplusblock
Train, prune and test a morphological neural network.
This is a companion code to the paper "Max-plus Operators Applied to Filter Selection and Model Pruning in Neural Networks" by Yunxiang Zhang, Samy Blusseau, Santiago Velasco-Forero, Isabelle Bloch and Jesús Angulo,
published in the International Symposium on Mathematical Morphology and Its Applications to Signal and Image Processing (ISMM) 2019.
https://link.springer.com/chapter/10.1007/978-3-030-20867-7_24
https://arxiv.org/pdf/1903.08072.pdf

Provided Tensorflow and Keras are installed, the code should be run by the command

python testMaxPlus.py

and needs the file maxPlusDense.py to work.
The script testMaxPlus.py defines a morphological neural network composed of an input layer, a linear layer and a max-plus (or dilation layer), trians it on the Mnist or fashion-mnist dataset, then removes the unused filters from the linear layer and finally tests the reduced network on the test set.
