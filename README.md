# Age-Gender-Classifier
An Age and Gender Classifier with a Fully-Connected artificial Neural Network


## Prerequisite

### Packages
For this work you will also need to install these Frameworks:
- Python 2 or 3
- [TFlearn](http://tflearn.org/installation/)

``
pip install tflearn
``

-	[Tensorflow](https://www.tensorflow.org/install/)

### Files and datasets
First, you should download the [Adience Dataset](http://www.openu.ac.il/home/hassner/Adience/data.html) (**faces.tar.gz (1.2Gb)** or **aligned.tar.gz (2.6Gb)** compressed files). 

You should also clone the [AgeGenderDeepLearning](https://github.com/GilLevi/AgeGenderDeepLearning) repository. Only the ***Folds*** repository will be necessary for the process; it contains the ***.txt files***, labels of the Adience Benchmark in separated age and gender files {***age_test.txt, age_train.txt, age_train_subset.txt, age_val.txt, gender_test.txt, gender_train.txt, gender_train_subset.txt, gender_val.txt***}.

Both files should be extracted and made available at the same location, otherwise ***make sure that the files paths are accessible from the Ipython Notebook files***. And also update the ***folds_path*** variable with the correct *Fold path name* and the ***images_root_directory*** variable with the correct Adience */face* or */aligned* repositories paths. This will ensure the creation of the ***Unified Dataset***.

Pay attention on the directory separators when writing the files' paths for Python 2 or Python 3. See the example below :

```python
if int(PyVersion[0])==2:
    folds_path='Age-Gender-Classifier/Folds/train_val_txt_files_per_fold' 
    print("Jean-Claude, I got in python 2")
else:
    folds_path='Age-Gender-Classifier\\Folds\\train_val_txt_files_per_fold'
    print("Jean-Claude, I got in python 3")
```

You could also instead clone this repository where the ***Folds*** directory is already available with Ipython Notebook files.

```
git clone https://github.com/Kjeanclaude/Age-Gender-Classifier.git
cd Age-Gender-Classifier/
# And also Extract the /face and/or /aligned datasets here.
```

And then simply execute the IPython Notebooks in your preferred environment.

```ipython
cd Age-Gender-Classifier/
jupyter notebook AgeGenderPrediction-OneHotModel.ipynb
# and/or
jupyter notebook AgeGenderPrediction-TuplesModel.ipynb
```

---
For more details, you should also find the proposal and the report PDF files on this repository.

---
### Roadmap

| Tasks | Date | Update |
| --- | --- | --- |
| Report | 30/06/2017 | 05/07/2017 |
| Write an example of prediction label interpretation function | 05/07/2017 | ... |
| Write an example of age prediction ranges function | ... | ... |
| Increase the Unified Dataset and make it available in a compressed file, with usage script | ... | ... |
| Provide a mobile app demo of the age and gender classifier | ... | ... |

---
---
```
==> "Intellectuals solve problems, geniuses prevent them."
==> "The difference between stupidity and genius is that genius has its limits."
```
[Albert-Einstein](http://www.movemequotes.com/top-21-albert-einstein-quotes/)
