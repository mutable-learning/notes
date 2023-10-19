tags:: Algorithmics
alias:: Reinforcement Learning

-
- how software agents ought to take actions in an environment so as to maximize some notion of cumulative reward
- an agent learns to behave in an environment by trial and error with the agent receiving rewards for taking actions that lead to desired outcomes, and punishments for taking actions that lead to undesired outcomes
- often use [[Dynamic Programming]] techniques
- training for reinforcement learning involves
	- an agent interacting with an environment
	- the agent takes actions in the environment and receives rewards or punishments for those actions
	- the agent then uses these rewards and punishments to update its policy, which is a mapping from states to actions
	- the goal of the agent is to learn a policy that maximizes the rewards it receives
- used for problems such as
	- Control problems
		- the goal is to control a system to achieve a desired outcome such as to train robots to perform tasks such as stacking blocks or playing a game of Pong
	- Planning problems
		- the goal is to find a sequence of actions that will lead to a desired outcome such as planning a route for a self-driving car or to schedule production in a factory
	- Games
		- used to train agents to play games
-
- Further Research
  background-color:: purple
	- Read
		- [Reinforcement learning - Wikipedia](https://en.wikipedia.org/wiki/Reinforcement_learning)
	- Watch
		- {{video https://www.youtube.com/watch?v=nIgIv4IfJ6s&pp=ygUWcmVpbmZvcmNlbWVudCBsZWFybmluZw%3D%3D}}
		- {{video https://www.youtube.com/watch?v=JgvyzIkgxF0&pp=ygUWcmVpbmZvcmNlbWVudCBsZWFybmluZw%3D%3D}}