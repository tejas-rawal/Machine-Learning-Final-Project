# Understanding the Amazon from Space
Kaggle Competition - https://www.kaggle.com/c/planet-understanding-the-amazon-from-space

## Using satellite data to track the human footprint in the Amazon rainforest.
Every minute, the world loses an area of forest the size of 48 football fields. And deforestation in the Amazon Basin accounts for the largest share, contributing to reduced biodiversity, habitat loss, climate change, and other devastating effects. But better data about the location of deforestation and human encroachment on forests can help governments and local stakeholders respond more quickly and effectively.

This goal of this competition is to label satellite image chips with atmospheric conditions and various classes of land cover/land use. Resulting algorithms will help the global community better understand where, how, and why deforestation happens all over the world - and ultimately how to respond.

## Dataset
This dataset contains 40,479 (RGB) satellite images, along with their associated labels.

Due to computation limits, only 5,365 images were used for this project.

### Training
The training set contains 3,755 satellite images, accounting for 70% of the total images.

### Test
The validation set contains 1,610 satellite images, the remaining 30% of the images.

## Models Trained

### Custom CNN
- A custom, sequential CNN model was built which included convolution, max pooling, dropout, and dense layers.
- There are ~4 million parameters in this model.

### ResNet50
- A pre-trained [ResNet50](https://www.tensorflow.org/api_docs/python/tf/keras/applications/ResNet50) model trained on the ImageNet dataset.
- Fine-tuned using transfer learning

## Results
To see results of the trained models, run the `Report.ipynb` notebook. Make sure to run and pass the `Notebook Setup` step first.

Results can also be viewed on [Google Colab](https://colab.research.google.com/drive/14uT-mqkm-0763lcoV17AHgHzxt28CdN-?usp=sharing)


