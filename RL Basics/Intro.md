# Intro

## What Is Reinforcement Learning?
Reinforcement learning (RL) is an area of machine learning that focuses on how you, or how some thing, might act in an environment in order to maximize some given reward. Reinforcement learning algorithms study the behavior of subjects in such environments and learn to optimize that behavior.

# Markov Decision Processes (MDPs) - Structuring A Reinforcement Learning Problem

## Components Of An MDP
Markov decision processes give us a way to formalize sequential decision making. This formalization is the basis for structuring problems that are solved with reinforcement learning.

In an MDP, we have a decision maker, called an agent, that interacts with the environment it's placed in. These interactions occur sequentially over time. At each time step, the agent will get some representation of the environment's state. Given this representation, the agent selects an action to take. The environment is then transitioned into a new state, and the agent is given a reward as a consequence of the previous action.

Components of an MDP:
- Agent
- Environment
- State
- Action
- Reward

This process of selecting an action from a given state, transitioning to a new state, and receiving a reward happens sequentially over and over again, which creates something called a trajectory that shows the sequence of states, actions, and rewards.

Throughout this process, it is the agent's goal to maximize the total amount of rewards that it receives from taking actions in given states. This means that the agent wants to maximize not just the immediate reward, but the cumulative rewards it receives over time.

## MDP Notation

We're now going to repeat what we just casually discussed but in a more formal and mathematically notated way.

In an MDP, we have a set of states **S**, a set of actions **A**, and a set of rewards **R**. We'll assume that each of these sets has a finite number of elements.

At each time step *t* = 0, 1, 2, ...,the agent receives some representation of the environment's state S
. Based on this state, the agent selects an action 
. This gives us the state-action pair 
.

Time is then incremented to the next time step 
, and the environment is transitioned to a new state 
. At this time, the agent receives a numerical reward 
 for the action 
 taken from state 
.

We can think of the process of receiving a reward as an arbitrary function 
 that maps state-action pairs to rewards. At each time 
, we have
The trajectory representing the sequential process of selecting an action from a state, transitioning to a new state, and receiving a reward can be represented as
This diagram nicely illustrates this entire idea.

