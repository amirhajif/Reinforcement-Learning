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


# SARSA(STATE-ACTION-REWARD-STATE-ACTION)
	1.	Initialization:
		•	Define all possible states and actions.
		•	Initialize  Q(s, a)  to 0 for all state-action pairs.
	2.	Update Rule:
		•	For each transition:
		Q(s, a) <- Q(s, a) + alpha.[ R + gamma.Q(s`,a`) - Q(s, a)]

	3.	Action Selection:
	•	Use an ε-greedy policy to balance exploration and exploitation.
	4.	Execution:
	•	Iterate through episodes, updating the Q-values for state-action pairs.
	
	Key Parameters:
	•	 \alpha : Controls how much new information overrides the old.
	•	 \gamma : Determines the weight of future rewards.
	•	 \epsilon : Probability of exploring random actions.