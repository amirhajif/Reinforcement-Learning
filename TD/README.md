# TD(0)
	1.	Initialization:
	•	Define a list of states.
	•	Initialize the value function  V(s)  for each state to 0.
	2.	Update Rule:
	•	For each transition, compute the TD target:

TD_target = R +gamma.V(s`)

	•	Compute the TD error:

TD_error = TD_target - V(s)

	•	Update the value function:

V(s) = V(s) + alpha.TD_error
