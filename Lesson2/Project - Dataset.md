# Create a Medical Image Annotation job

## Project overview
==Goal==: **build a product that helps doctors quickly identify cases of pneumonia in children.

> *You should design a data annotation job, such that a non-expert can identify more noticeable cases of pneumonia. Since you are designing for a non-expert annotator, you should design for failure; this means including some way to capture uncertainty in your data labels and test questions.*

- it will be a classification system
	- Focused on quickly identifying healthy patients and surfacing potential cases
	- Not meant to be a replacement for a doctor
- The main task is to create a data labeling job using #Append

### The submission
1. An ==HTML file of a complete job Preview==
	1. Instructions for annotation
	2. Example test questions
2. A ==proposal document== that discusses the design of the job and steps to perform quality assurance.
	1. Discuss your design choices and methods

#### The dataset
is a modified version of the [Chest X-Ray images (Pneumonia) in Kaggle](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia).

![](https://video.udacity-data.com/topher/2019/April/5cae622b_annotated-chest-xray/annotated-chest-xray.png)

#### What does indicate pneumonia?
- **Normal**:
	- Clear lungs (no  cloudiness/opacity areas)
	- Web-like vasculature in the lungs may be presented.
	- You could see a diaphragm shadow at the bottom
- **Pneumonia**:
	- Areas of cludiness/opacity =>
		- Several concentrated areas
		- A large area

#### Good Annotator Instructions
- Include an `Unknow` or `other` option to account for uncertainty in annotation.
- Maybe include a numerical scale to let the annotator choose how likely he think a case of pneumonia is in a given image.


## Creating a job with Append

1. Create an Append Account
    1. jricci@cicese.edu.mx
    2. 53rest0$Patr0nu$
2. The job Creation page.
	1. Follow the steps mentioned in the [[Creating a Dataset]] note


## Project Materials
