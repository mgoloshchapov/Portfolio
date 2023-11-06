### CNN classification of Ising model temperature

I use TensorFlow to implement Convolutional Neural Network(CNN)
for Ising model temperature classification. Follow [this link]() for notebook with code.

<p align="middle">
  <img src="./images/ising_confusion.jpg"/>

  <p align="center">
    Fig. 1: Confusion matrix for temperature classification. Red box highlights temperature close to phase transition.
  </p> 
</p>

Dataset for ~50k images is generated using single-spin-flip Monte-Carlo.

<p align="middle">
  <img src="./images/ising_predict.jpg"/>

  <p align="center">
    Fig. 2: Classification of temperature for different spin configurations.
  </p> 
</p>

Spin configurations are also rotated and reflected to enlarge the dataset(x8).

<p align="middle">
  <img src="./images/rotations.png"/>

  <p align="center">
    Fig. 3: Modification of configurations to make dataset larger. 
  </p> 
</p>




