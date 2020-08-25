# 2 layer neural network
* implement a 2 layer neral network without any libraries and from scratch.
* using mnist handwritten numbers dataset.
* label numbers greater than or equal to 5, to 1 and less than 5, to 0. 

# Steps

### Activation Function
* #### sigmoid(z) = 1/(1+<img src="https://render.githubusercontent.com/render/math?math=e^{-z}">)


### Initialize Parameters
* #### For a 2-layer NN we need W1, b1, W2 and b2

* #### W[L].shape = (no. of nerons in layer L, no. of nerons in layer L-1)


### Forward Propagation
* #### Compute Z1, A1, Z2 and A2(y)

* #### Z1 = W1.X+b1

* #### A1 = sigmoid(Z1)

* #### Z2 = W2.A1+b2

* #### A2 = sigmoid(Z2)


### Loss Function
* #### Loss(Y-hat, Y) = <img width="" height="30" src="https://render.githubusercontent.com/render/math?math=\frac{-1}{m} \sum_{k=1}^{m}{}"> log(Y-hat).Y + (1-Y).log(1-Y-hat)

* #### m : number of samples

### Back Propagation
* #### Compute gradients of W1, b1, W2 and b2 as dW1, db1, dW2 and db2


### Update Parameters
* #### Update W1, b1, W2 and b2 using a learning rate and dW1, db1, dW2 and db2

* #### W1 = W1 - leraning-rate * dW1

* #### b1 = b1 - leraning-rate * db1

* #### W2 = W2 - leraning-rate * dW2

* #### b1 = b1 - leraning-rate * db2
