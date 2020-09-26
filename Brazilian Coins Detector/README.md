# Brazilian Coins Detector<br/>
## Detect brazilian coins of 5 classes: 5, 10, 25, 50, 100<br/>
* Dataset from Kaggle: Brazilian Coins - Classification set. <a>https://www.kaggle.com/lgmoneda/br-coins?select=classification_dataset</a><br/>
* ### The configurationg of CNN:<br/>
    * Convolutional Layer 2D with 32 5x5 feature, activation function = "relu"
    * Max Pool layer of 2x2
    * Convolutional Layer 2D with 64 3x3 feature, activation function = "relu"
    * Max Pool layer of 2x2
    * Convolutional Layer 2D with 128 3x3 feature, activation function = "relu"
    * Max Pool layer of 2x2
    * Convolutional Layer 2D with 128 3x3 feature, activation function = "relu"
    * Max Pool layer of 2x2
    * Dropout set to 20%
    * Flatten
    * Fully connected(Dense) layer with 128 units, activation function = "relu"
    * Fully connected(Dense) output layer 5 units, activation function = "softmax"
    * Optimizer = "Adam"
    * Loss Function = "categorical_crossentropy"
* ### Optimization:
    * To impove the accuracy of the model:<br/>
      #### Step 1:<br/>
          Detect the coin in images and crop the coin
      #### Step 2:<br/>
          Augment the dataset images using ImageDataGenerator library
* ### Result:<br/>
    * Finally, we got an accuracy of around 95%
