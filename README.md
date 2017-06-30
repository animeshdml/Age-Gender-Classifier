# Age-Gender-Classifier
An Age and Gender Classifier with a Fully-Connected artificial Neural Network


## Prerequisite

### Files and dataset
First, you should download the [Adience Dataset](http://www.openu.ac.il/home/hassner/Adience/data.html) (**faces.tar.gz (1.2Gb)** or **aligned.tar.gz (2.6Gb)** compressed files). 

You should also clone the [AgeGenderDeepLearning](https://github.com/GilLevi/AgeGenderDeepLearning) repository. Only the ***Folds*** repository will be necessary for the process; it contains the ***.txt files***, labels of the Adience Benchmark in separated age and gender files {***age_test.txt, age_train.txt, age_train_subset.txt, age_val.txt, gender_test.txt, gender_train.txt, gender_train_subset.txt, gender_val.txt***}.

Both files should be extracted and made available at the same location, otherwise ***make sure that the files paths are accessible from the Ipython Notebook files***. And also update the ***folds_path*** variable with the correct *Fold path name* and the ***images_root_directory*** variable with the correct Adience */face* or */aligned* repositories paths. This will ensure the creation of the ***Unified Dataset***.

You could also instead clone this repository where the ***Folds*** directory is already available with Ipython Notebook files.

``
git clone https://github.com/Kjeanclaude/Age-Gender-Classifier.git
``

And then simply execute the IPython Notebooks in your preferred environment.

### Packages
For this work you will also need to install these Frameworks:
- Python 2 or 3
- [TFlearn](http://tflearn.org/installation/)

``
pip install tflearn
``

-	[Tensorflow](https://www.tensorflow.org/install/)
