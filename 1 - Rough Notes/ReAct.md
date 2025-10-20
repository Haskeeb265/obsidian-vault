
2025-10-19 23:21

Status: #InProgress 

Tags: [[AI]] 

# ReAct

- Chain of thoughts are good but they can only work on their internal representation
- Recent works use long prompt initialization(?) to ground the model however in the long run it eventually fails
- **ReAct = (Reason + Act)**
- Reasoning = "How to solve the problem?"
- Act = "Solving the problem with the help of given tools?"
- ReAct enables language models to generate both verbal reasoning and text actions in an **interleaved** manner
- Actions lead to observation feedback
- Previous models could either do reasoning OR act. ReAct enables models to do both at the same time

#### Flow of ReAct
LM => Reasons + Corrects reasoning by itself
LM => Performs an Action 
								=> Action is given a feedback by an external observation 
									=> LM improves the the Action in the next runs

ReAct enables the model to perform all of the above tasks at the same time


- Where reasoning is of primary importance, ReAct allows the model to perform as many corrections as possible and vice versa if action is of more importance.
- 


#### References
[[ReAct Synergizing Reasoning and Acting in Language Models]]