# age_gender_classification
This project aims to classify gender and age of person.

### Dataset Description
In order to facilitate the study of age and gender recognition, they provide a data set and benchmark of face photos. The data included in this collection is intended to be as true as possible to the challenges of real-world imaging conditions. In particular, it attempts to capture all the variations in appearance, noise, pose, lighting and more, that can be expected of images taken without careful preparation or posing. This dataset is known as Adience Benchmark Dataset.
Dataset is divided in 5 folds and 4 folds are taken as train and 5th is used as validation data. There are 14047 images for train and 3445 images for test.

### Tools and Libraries 
  - Numpy
  - Pandas 
  - Keras
  - Tensorflow

### Approach 
  - Age and Gender Classification using transfer learning with VGG19 architecture and weights of imagenet, this model achieved validation accuracy of 57.2% on age classification and 89.1% on gender classification. These results are better than that in paper https://www.openu.ac.il/home/hassner/Adience/EidingerEnbarHassner_tifs.pdf

  - Another approach used is to extract the features of images using VGG19 architecture and imagenet weights and then used boosting tree classifier, we tried LightGBM Classifer and got 50.2% validation accuracy score on age and 86.7% score on gender classification.

  - Can use variational Encoder for classification but that requires high computation.
  
  - Used Data preprocessing methods such as croping and aligning using MTCNN and DLib but they were not of much help.
  
### Future Works
  - Deployment on the web 



