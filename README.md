# Deep Learning project - Document classification 
This repository contains the project made for the course **Deep Learning in Practice with Python and LUA** (**BMEVITMAV45**) by <em>KornĂŠl TĂłth (AE92AW) </em>, <em>Zsolt Bartis (E4E2QK) </em>, <em>BĂĄlint Gyimes (Y46RYU) </em>

## Dataset
For the training, the DBpedia dataset was used, which was obtained from the [source](https://drive.google.com/uc?export=download&id=0Bz8a_Dbh9QhbQ2Vic1kxMmZZQ1k) provided in pythorch documentation. 

The DBpedia ontology classification dataset is constructed by picking 14 non-overlapping classes from DBpedia 2014. They are listed in classes.txt. From each of thse 14 ontology classes, we randomly choose 40,000 training samples and 5,000 testing samples. Therefore, the total size of the training dataset is 560,000 and testing dataset 70,000.
The files train.csv and test.csv contain all the training samples as comma-sparated values. There are 3 columns in them, corresponding to class index (1 to 14), title and content. The title and content are escaped using double quotes ("), and any internal double quote is escaped by 2 double quotes (""). There are no new lines in title or content.
Some of the class names are: Company, EducationalInstitution, Artist, Athlete

## Description
The main role of this project is to create a neural network for document classification. As a first approach, only 5 classes are used to build networks. After that, the accuracy of classification is investigated after adding further classes to the dataset. Two ways of training are considered: based on multiple datasets, where the titles and the articles are different datasets, and based on a single dataset, after merging the title with the article. The difference of the two ways of training is investigated. 

## Usage
The current, up-to-date version of the code is located in the <code>fitting_test.ipynb</code>. At this point we train a basic model with only the titles from the used dataset.
To train the model run all the cells in the following blocks designated by the corresponding markdown cells:
- Importing datasets
- Pre-processing
- Model and fitting

After the fitting is finished or the saved weights from the <code>model.hdf5</code> file are loaded the evaluation can be acquired by running all the cells in the Evaluation block.
Toucan
Over 100 word limit
We’re working to increase this limit and keep load times short. In the meantime, try highlighting up to 100 words at one time to translate.
Don’t show again
