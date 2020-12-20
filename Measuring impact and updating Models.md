## **Introduction to business impact**
- Benefits and challenges of AI initiatives
- Define and measure success metrics
- A/B testing and versioning
- Monitor and mitigate bias
- Continuous Learning
- Scale
- Compliance & ethics

## **Measuring success**
### Success metrics
**Consider:**
- Customer experience
- Revenue gain
- Customer engagement
- Business process automation
- Better & faster decision making

### Outcome vs output
==Focus on outcome and not output==
**Outcome:** What we want
- Generate Revenue
- Improve Customer experience
- Automate and save cost

**Output:** A metric to track
- Accuracy
- Execution time
- Recall
- Precision

### Key Success Metrics
| Vanity metrics                   | Business metrics            |
| -------------------------------- | --------------------------- |
| Number of active users           | Conversion rate             |
| Number of bot sessions initiated | Customer support savings    |
| Average chat sessions            | Increase Net Promoter Score |
| Average chats handled by bot     | Cost per acquisition        |

- Net Promoter Score (NPS):
	- Calculated based on the response to a single question: *How likely is it that you would recommend our XXX to a friend or colleague*
- Cost per acquisition (CPA):
	- Is an online adverising pricing model where th adveriser pays for a s pecified acquisition 

#### Measure => Learn => Evolve

## A/B Testing & Versioning
### A/B testing model
![[Captura de Pantalla 2020-12-16 a la(s) 22.18.20.png]]
Two models:
	- Send about 20% of the customers to a new model => **Challenger** model.
	- 80% to a well-tested model => **Controled model**

**Best A/B testing practices:**
	- Deciding on a performance metric
	- Deciding on test type based on your performance metric
	- Choosing a minimum effect size you want to detect
	- Determining the sample size
	- Running the test until sample size is reached
	
**Thing to consider**:
- Cost benefit analysis
	- Is x% accuracy gain beneficial for business?
	- Does a slightly improvement requires a high investment?
- Run the test long enough to capture any seasonality effects
- Control the experiment to avoid "novelty effect"
	- initial positive reaction that wears off

### Monitor Bias
#### Different types of bias
1. Model Bias:
	- The model itself generates bias outcome
2. Annotation bias
	- Introduced by humans
3. Data bias
	- Unbalance selection of source data

#### Addressing Unwanted Bias
- How to solve unwanted bias?
	1. Awareness
		- Defining the decision you are asking your model to solve for
		- Is the decision simple, with black and white answers?
		- Real-worlds scenarios always have context
		- Is there a protected class or status involved in this decision?
	2. Data, data, data...
		- Where do you get your source data?
		- Could there be a sourcing bias?
		- Cover for enough examples and edge cases
		- Think about all your end-users and test with them
		- Structure Data gathering that allows for difference of opinions:
			- Gather a diverse ML team that asks diverse questions
			- Annotate with diversity
	3. Iterate and Learn
		- Be transparent on what data the system is trained on and its limitations
		- Be empathetic and understand that your end-users will use the system differently.
		- Take feedback and have opinions
		- Ensure that the system is actively learning

## Continuous learning
- Involves a feedback loop between humans and the model
	- When low confident predictions -> Send to humans for annotation -> retrain the model
	- Continue until get high confident predictions
	- Perform smart selection for annotation

#### Smart Selection
- Identify the most valuable training data units for human annotation
- It takes four criterias:
	1. Low confidence: Any datatype challenging the model
	2. Uncertainty: Scenarios when the model is not able to predict
	3. Novelty: Any new data
	4. Class importance: Identify the classes important to the model

#### Model Staleness
- The performance of the model decreases over time

## Privacy-first Approach
![](https://video.udacity-data.com/topher/2019/May/5cef0185_polaris-consent/polaris-consent.jpg)

## Scaling a product
### Organize for Scale
- Machine Architecture
- ![[Captura de Pantalla 2020-12-18 a la(s) 20.48.18.png]]
- Organization structure
