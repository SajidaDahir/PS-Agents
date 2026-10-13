Practical Exercise 3: Designing a Searching Agent

Agent: Self-Driving Trailer
Environment: Kenya's Highway Network
Initial State: Nairobi
Goal State: Kisumu

1. Introduction
- A problem-solving agent is a goal-based agent that searches for a sequence of actions that will lead it from the initial state to the goal state. The agent in this exercise is a self-driving trailer that travels through Kenya's highway network to find a route that minimizes the total travel distance.

1.1 PEAS Description
- Performance Measure - Reach Kisumu safely, minimize total distance travelled, avoid collisions, obey traffic regulations and complete the journey efficiently.
- Environment - Kenya's highway network, towns, junctions, pedestrians, traffic conditions, road signs and weather conditions.
- Actuators - Brakes, Indicators, accelerator, horn, accelerating system
- Sensors - GPS, cameras, radar, speed sensors

1.2 Agent Environment
- Fully observable VS Partially Observable - the environment is partially observable because the trailer's sensors cannot provide complete information about every aspect of the road environment at all times.
- Deterministic VS  Stochastic - the environment is stochastic because the outcome of an action may be affected by factors beyond the agent's control such as drivers, accidents and unexpected road conditions.
- Episodic VS Sequential - the environment is sequential because the agent's current decisions affect the subsequent states and available actions.
- Static VS Dynamic - the environment is dynamic because traffic, road and weather conditions may change while the agent is deciding which action to take.
- Single-Agent VS Multi-Agent - the environment is multi-agent since other road users such as drivers and pedestrians also act within the same environment, influencing the driver's decisions

2. Problem Formulation and Search
- Initial state: Nairobi
- Goal state: Kisumu
- State Space: Consists of the towns in the road network
- Available Actions: road connections that allow the trailer to travel from its current town to another town.
- Goal Test: it checks whether the current state is Kisumu.
- Path Cost Function: total road distance travelled from Nairobi to the current town.
- Transition Model: moving along a selected road leads to the connected town
- Optimal Solution: a valid route from Nairobi to Kisumu with minimum total road distance.

3. Abstraction of The Road Network
- The real-world road network is simplified by representing towns as states and direct road connections as edges.

