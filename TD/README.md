# TD(0)
	1.	Initialization:
	•	Define a list of states.
	•	Initialize the value function  V(s)  for each state to 0.
	2.	Update Rule:
	•	For each transition, compute the TD target:

TD\_target = R + \gamma \cdot V(s{\prime})

	•	Compute the TD error:

TD\_error = TD\_target - V(s)

	•	Update the value function:

V(s) = V(s) + \alpha \cdot TD\_error
