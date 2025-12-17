
2025-12-17 10:35

Status: #Finished
Tags: [[AI]] [[agents]]
# Reflexion

- A design pattern which allows agents/models to improve themselves without the need for fine tuning.

- Consists of 3 LLM based components:
	1. Actor = Generates an action
	2. Evaluator = Scores trajectories (thinking, reasoning, actions, final outcome) using Binary Feedback (Yes or no), Scalar feedback (you get a score), heuristic feedback,  
	3. Self-Reflection Model = It generates a basic natural language summary that tells the actor what it did wrong last time so it can be careful of that problem in the future.




#### References
