
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





#### References
[[ReAct Synergizing Reasoning and Acting in Language Models]]