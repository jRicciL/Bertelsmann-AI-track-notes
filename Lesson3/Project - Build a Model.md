## Project preview
**Build a product that helps doctors quickly identify cases of pneumonia in children**

### Goals:
- Help flags ==serious cases==
- Quickly identify healthy cases
- Act as a diagnostic aid for doctors

### Task
Classify images of childrens' chest x-ray images => 
- Normal
- Pneumonia

### General procedure
- We are going to use Google AutoML
- We will build models with 4 variants of the data set

### What will be graded 
- The ability to build a model using Google's AutoML Vision platform
- Understand how properties of data impact performance of models

### The data
-  [Kaggle chest x-ray dataset](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)

### Four parts of the project
1. ==Create a **binary classifier** to detect pneumonia using chest x-rays==. Train a model using 100 images from "normal" and 100 images from "pneumonia" classes.
	- **Train/Test split:** *how much data is used for training and how much is used for testing?*
	- **Confusion matrix**: *What do each of the cells in the confusion matrix describe?*
	- **Precision & Recall**: *What do these measure and how are they calculated?*

2. ==Create an **unbalanced binary classifier**==. Use 100 images from "normal" and 200 from "pneumonia".
	- **Confusion matrix**: What does the confusion matrix tell you about unblanced data?
	- **Precision & Recall:** How are precision and recall affected?
	- **Unbalanced classes**: How do unbalanced classes impact a machine learning model?

3. ==Create a **binary classifier with dirty data**==. Start with 100 and 100 images of each class => Switch the labels of 30 images in each class => 30% of data mislabeled
	- **Confusion matrix**: *How is the confusion matrix affected?*
	- **Precision & recall:** *How are precision and recall affected?*
	- **Dirty data:** *How do dirty data impact the model?*

4. ==Create a **three-class model** with the classes "normal", "bacterial pneumonia", and "viral pneumonia"== The labels are present in the image filenames. Use 100, 100 and 100 of each class.
	- **Confusion matrix:** *What does the 3-class confusion matrix look like?*
	- **Precision & recall:** 
		- *What are the model's precision and recall?* 
		- *How are these measures calculated?*
	- **More data: **
		- *Can you continue to add data to each class (while keeping the data balanced) and get the model to 85% precision and recall?*
		- *How many data did you end up using?*

## AutoML modeling report
- [AutoML Modeling Report](https://video.udacity-data.com/topher/2019/October/5daac1f3_automl-modeling-report-all-fixed/automl-modeling-report-all-fixed.docx)