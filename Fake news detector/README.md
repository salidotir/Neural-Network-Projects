# Fake news detector

## Introduction
We are going to create a model for detecting fake news with 3 ways:
* Decision trees
* K-Fold cross validation
* Random forest

## Use
* Go to Collab
* Download input dataset into your google drive
* Mount your google drive to access dataset
* Edit below code to write the path of your input data instead of *path-in-google-drive* to copy these 2 datasets into virtual hard disk to use:

  ```python
  !cp "path-in-google-drive/pol-fake.csv" "/content/sample_data"
  !cp "path-in-google-drive/pol-real.csv" "/content/sample_data"
  ```
  
## Results
* Decesion tree using *gini* method: **accuracy: 64.42%**
* Decesion tree using *information gain* method: **accuracy: 65.77%**
* Random Forest: **accuracy: 75.16%**
