
## Overview of Modeling
### Concepts
- Overview of modeling
- Training Data
- Model Evaluation
- Transfer learning and Automated Machine Learning

#### Modeling key points
- Neural networks are a series of layers comprised of computational nodes
- Activation functions act as decision boundaries for a node
- Weights on the inputs are tuned during training
- Different node types and architectures are used for specific problem types


## Neural Networks 
- First developed in 1950
- A series of computational layers
- Specialized nodes perform various computations
- ![](https://video.udacity-data.com/topher/2019/May/5cee1b8e_neuron-in-out/neuron-in-out.gif)
- The structure of how the nodes and layers are connected is know as network's architecture

### Activation Functions
- Serve as the decision boundary to pass information
	- by performing nonlinear transformations to the flowing data
- An ideal activation function will return a range of values rather than a binary output

#### Examples
| Activation Function | Decision              | Boundaries  | Features              |
| ------------------- | --------------------- | ----------- | --------------------- |
| Step Function       | 1 if x > k, else 0    | 1 -> 0      |                       |
| Sigmoid Function    | 1 / (1 + e^-x)        | 1 -> 0      | Soft                  |
| ReLU                | x if x > 0, else 0    | 0 -> inf    | Fast                  |
| Leaky ReLU          | x if x > 0, esle a\*x | -inf -> inf |                       |
| Linear Function     | x = cx                | -inf -> inf | Proportional to input |
| Tanh Function       | (2/(1 + e^(-2x))-1)   | -1 -> 1            |                       |



### Backpropagation and & updating the weights of a network
- During training.
	- The NN starts off randomly guessing the appropriate weights.
	- Then the model make predictions and compare them against the observed values.
		- Thus, the model is able to measure is ==Error==
- For a model to ==improve== it needs to:
	1. Identify the source of its error => Which model weights are responsible for the error?
	2. update those weights to a new, better value.
- The previous steps are done during the **backpropagation** phase.
	- The process consists on going backward through the modes and layers to find the source of error.
	- then, the weights are updated => Their value change in response to the error


There are different types of nodes and networks specialized in various use cases

## Data in Machine Learning
### Training data
- Data defines model behavior and performance
- Model parameters are updated based on training data
- A model will not learn if it's not in the data
- ==Bad data -> Bad model==

#### Training data is key
- Data used to train a model should reflect real-world data
- Diverse data set => More robust model
	- Data that encompasses all likely scenarios
	- Photos from the real world
	- Equal amounts of the different types of data
	- Correctly labeled data
	
#### Common issues with training data
- Unbalanced or biased data
- Training data differs from real data
- Mislabeled data

### Model Evaluation 
- ** #Precision** = True positives / Model predictions
	- Measure the percentage of correct predictions against total number of predictions
	- *How many of the predicted objects are correct?* =>
- ** #Recall** = True positives / Really true positives
	- Measures the percentage of correctly identified instances from the total possible instances
	- *How many of the Real positives the model found?*
	- *How good is the model at identifying actual occurrences of objects in the data?*
![](https://www.kdnuggets.com/images/precision-recall-relevant-selected.jpg)
- **F1 Score**: #F-score
	- Combines the precision and the recall
		- It is the harmonic mean of precision and recall
		- $F_1 = \frac{2} {recall^{-1} + precision^{-1}} = 2 \cdot \frac{precision \cdot recall}{precision + recall}$
	- It represents and overall measure of the model's performance

- **Confusion Matrix**

## Transfer Learning and Fine Tuning
- Use the knowledge from an already trained model with a similar use case
	- The architecture and parameters of the network are adapted to our case
	- Allow us to develop models with less data required

#### Transfer Learning Procedure
- Take the already trained network
- Reduce the time and amount of data required to train a new network
- Common procedure in #image-classification
	- Because the first layers tend to be responsible for identifying general patterns in shape and color, such as simple lines and textures.
- Copy the layers to use the same architecture (except the output layer) => to keep:
	- The same architecture
	- The same weights
	- The same activation functions
- Adapt the new output layer of the new model
- ==**Only retrain the last layer of the new model**== #Transfer-Learning
	- Original weights are preserved

#### Fine Tuning
- in #Fine-tuning we use the same process as with #Transfer-Learning but the earlier layers are also **retrained**

## Automated ML
- Let us to create robust and scalable models without much Machine Learning Experience
- Cloud services offer the opportunity of create models from data in an easy manner
	- Allows for quick prototyping
	- Benefit of enterprise support
	- Much less hassle and complexity

#### Neural Architecture Search
- They Automatically determine the best architecture form data
- Consists of architecture blocks that can be configured for optimization
![[Captura de Pantalla 2020-12-13 a la(s) 15.38.45.png]]
