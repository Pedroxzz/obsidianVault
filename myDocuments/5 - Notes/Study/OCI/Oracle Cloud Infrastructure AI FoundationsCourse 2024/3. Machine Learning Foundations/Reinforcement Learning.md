---
tags:
  - oci
Index: "[[3. Machine Learning Foundations]]"
---
# Transcript 
In this lesson, we will learn about reinforcement learning. Reinforcement learning is like teaching a dog new tricks. You reward it when it does something right. And over time, it learns to perform these actions to get more rewards.

More formally, reinforcement learning is a type of machine learning that enables an agent to learn from its interaction with the environment, while receiving feedback in the form of rewards or penalties without any label data. Let us look at some examples.

Reinforcement learning is more prevalent in our daily lives than we might realize. To name a few, autonomous vehicles, the development of self-driving cars and autonomous drones rely heavily on reinforcement learning to make real-time decisions based on sensor data, traffic conditions, and safety considerations. Smart home devices. Virtual assistants like Alexa, Google Assistant, and Siri, utilize reinforcement learning to improve natural language processing and adapt to individual users speech patterns and preferences.

Industrial automation. In manufacturing and production processes, Reinforcement learning is applied to optimize the performance of robots and control systems, leading to improved efficiency and reduced service. Gaming and entertainment. Mini video games, virtual reality experiences, and interactive entertainment use reinforcement learning to create intelligent and challenging computer controlled opponents. The AI characters in games learn from player interactions and become more difficult to beat as the game progresses.

Let us take an example to discuss common terminology. Let us say we want to train a self-driving car to drive on a road and reach its destination. For this, it would need to learn how to steer the car based on what it sees in front through a camera.

In this example, car and its intelligence to steer on the road is called as an agent. More formally, agent is a learner or decision-maker that interacts with the environment, takes actions, and learns from the feedback received. Environment, in this case, is the road and its surroundings with which the car interacts. More formally, environment is the external system with which the agent interacts. It is the world or context in which the agent operates and receives feedback for its actions.

In this example, what we see through a camera in front of a car at a moment is a state. More formally, state is a representation of the current situation or configuration of the environment at a particular time. It contains the necessary information for the agent to make decisions. The actions in this example are to drive left or right or keep straight.

Formal definition of actions, actions are a set of possible moves or decisions that the agent can take in a given state. Actions have an impact on the environment and influence future states. After driving through the road many times, the car learns what action to take when it views a road through the camera. This learning is a policy. Formally, policy is a strategy or mapping that the agent uses to decide which action to take in a given state. It defines the agent's behavior and determines how it selects actions.

Consider the example of training a dog to learn tricks like pick up a ball, roll, sit, and so on. Here the dog is an agent, and the place it receives training is the environment. While training the dog, you provide a positive reward signal if the dog picks it right and a warning or punishment if the dog does not pick up a trick. In due course, the dog gets trained by the positive rewards or negative punishments.

The same tactics are applied to train a machine in the reinforcement learning. For machines, the policy is the brain of our agent. It is the function that tells what actions to take when in a given state. The goal of reinforcement learning algorithm is to find the policy that will yield a lot of rewards for the agent if the agent follows that policy, referred to as the optimal policy. Through a process of learning from experiences and feedback, the agent becomes more proficient at making good decisions and accomplishing tasks.

This process continues until eventually we end up with the optimal policy. The optimal policy is learned through training by using algorithms like Deep Q Learning or Q Learning Let us explore this a little more with another example.

Reinforcement learning can be used in a robotic arm to optimize the process of placing goods in a warehouse. The goal is to teach the robotic arm how to pick up items and place them efficiently and accurately in the desired locations within the warehouse. Let us see how a robotic arm gets trained using reinforcement learning.

The first step is setting the environment. This includes the robotic arm, the warehouse layout, the goods to be placed, and the target locations for each item. The second step is to define state representations. For the robotic arm, the state can include information such as the position and orientation of the arm, the position of the items to be picked up and the positions of the target locations.

Next is action space. Define the action space. Action spaces are the possible actions the robotic arm can take in each state. Decide rewards and penalty. The robotic arm should be rewarded when it successfully places an item in the correct location and penalize for dropping items, damaging goods, or failing to place items accurately.

In training, the robotic arm starts in a random state and takes actions in the environment. Initially, it explores different actions randomly and observes the rewards and penalties it receives for each action. As it learns, it starts to prioritize actions that lead to higher rewards and avoids actions that result in penalties. Through multiple training iterations, the robotic arm learns better strategies for picking up and placing items in the warehouse. Thanks for watching.