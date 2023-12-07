# SHD_Linear_Separability

Welcome to this repository where you'll get to tackle a Keyword Spotting dataset with Logistic Regression and still be able to get on the task's leaderboard.
We'll use the Spiking Heidelber Dataset (SHD) from https://zenkelab.org/resources/spiking-heidelberg-datasets-shd/
It's a dataset targeting Spiking Neural Networks, as the speech recordings of 20 spoken digits (0 to 9 in english and 0 to 9 in german) are translated into spike trains (feature vectors of 0s and 1s).

The spirit of the task is to process such data in a streaming fashion, thus one time-step at the time. However, here we investigate what happens when considering the temporal dimention as a normal fearure vector. We store the temporal evolution of the input in memory and process it altogether.
First, we will apply a linear classification algorithm, to look at the Linear Separability of the dataset. Surprisingly, we'll reach 92.4% classification accuracy in the test set, ranking such approach in the 4th place on the leaderboard.
Then, we'll try with a Multi-Layer Perceptron and a Convolutional Neural Network to try and break the State-of-the-Art accuracy. A CNN with as little as 30k parameters will score at 97.4%, reaching the highest performance in the leaderboard to date.

Obviously, more complicated models are likely to perform even better. You are welcome to contribute in this direction and explore larger CNNs or even Vision Transformers! But remember, all of this is just for fun. The spirit of the task is to process the input information in a sequential manner.
Enjoy the notebook,
Filippo
