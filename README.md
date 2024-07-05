# Application of complex networks to analyze how cooperation is influenced by network topology

In the context of complex networks, 'Cooperation' is a field of study that explores how individual agents (such as people, organizations, or biological entities) interact and collaborate in interconnected and dynamic systems.

Furthermore, the topology of a complex network refers to the structure and organization of connections (edges) between the elements (nodes) of the network. It is essentially the "map" of how nodes are connected to each other. The topology of a complex network can significantly influence the behavior and dynamic properties of the network.

The project in this repository seeks to understand how different topologies (Erdős-Rényi, Watts-Strogatz and Barabási-Albert) can stimulate the cooperation of the agents involved.

To this end, simulations were carried out using a model based on the iterated prisoner's dilemma, a game widely used to study cooperation in dynamic systems. The iterated prisoner's dilemma allows us to analyze how cooperation can emerge and sustain itself in an environment where agents have the option to cooperate or betray (defect) in each interaction.

## Methodology
### Network Generation:

- Erdős-Rényi: Randomly generated networks where each pair of nodes has the same probability of being connected.
- Watts-Strogatz: Small-world networks that introduce randomness into a regular network, allowing the presence of short global paths and high local clustering.
- Barabási-Albert: Scale-free networks where some nodes (hubs) have many connections, while the majority have few, following a power law distribution.

### Implementation of the Cooperation Model:

- Each node in the network represents an agent who can choose between cooperating or betraying.
- Interactions between agents are determined by the connections (edges) of the network.
- The temptation to cheat is an adjustable parameter that influences agents' decision to cooperate or not.

### Simulations:

- Carrying out multiple iterations for each type of network and parameter configuration.
- Monitoring the fraction of cooperating agents over time.
- Variation of temptation to defection to analyze its impact on cooperation.

## Results
### Erdős-Rényi Networks:

Cooperation tends to decrease rapidly as the temptation to defection increases. These networks show less robustness to cooperation compared to other topologies.


### Watts-Strogatz Networks:

They present greater robustness for cooperation, maintaining relatively high levels of cooperation even with increases in the temptation to defection. The small-world structure makes it easier to maintain cooperative clusters.

### Barabási-Albert Networks:

Networks with linear and sublinear growth show high robustness to cooperation, maintaining high levels of cooperating agents even under high temptation for defection.
Networks with superlinear growth, on the other hand, show significantly lower robustness to cooperation.

# Conclusions
This project demonstrated that network topology has a significant impact on the ability of a network to maintain high levels of cooperation between its agents. Linear and sublinear Barabási-Albert networks are the most efficient in sustaining cooperation, while Erdős-Rényi networks are the least efficient. Watts-Strogatz networks occupy an intermediate position, combining characteristics of both types of networks.

The results suggest that when designing systems and networks to maximize cooperation (such as in social networks, collaborative systems, and biological ecosystems), the choice of topology is crucial. Networks with well-connected hubs (such as Barabási-Albert) can provide a more robust framework for cooperation, especially when the temptation to defection is high.

# Possible practical applications
- Social Networks: Understand how the structure of social networks can promote collaboration and reduce negative behaviors.
Organizations: Design organizational structures that encourage cooperation among employees.
- Ecosystems: Understand how different species interact and collaborate in an ecosystem.

# References
- Prof.'s playlist Francisco Rodrigues in brazilian portuguese (also responsible for the material taught in person at ICMC-USP): https://www.youtube.com/playlist?list=PLSc7xcwCGNh0HHNJlZBMBK6MzpdwNSzVT
- Cardillo, Alessio & Gómez-Gardeñes, Jesus & Vilone, Daniele & Sánchez, Angel. (2010). Coevolution of strategies and update rules in complex Prisoner's Dilemma networks. New Journal of Physics. 12. 103034. 10.1088/1367-2630/12/10/103034.
- Poncela, J., Gómez-Gardeñes, J., Floría, L. M., & Moreno, Y. (2007). Robustness of cooperation in the evolutionary prisoner's dilemma on complex networks. New Journal of Physics, 9(6), 184. [doi: 10.1088/1367-2630/9/6/184]