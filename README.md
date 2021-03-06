# cart-and-pole-balancing
using reinforcement learning to solve the balance of cart and pole problem
The DQN(Deep Q network)is used along with reinforcement learning algorithm to train the agent the efficiently in order to reach the cummulative maximum rewards at the end of the epiosde.
The DQN class has been extended from nn.module
steps involved in combining Deep Q network with reinforcement learning.
Initialize replay memory capacity.
Initialize the policy network with random weights.
Clone the policy network, and call it the target network.
For each episode:
Initialize the starting state.
For each time step:
Select an action.
Via exploration or exploitation
Execute selected action in an emulator.
Observe reward and next state.
Store experience in replay memory.
Sample random batch from replay memory.
Preprocess states from batch.
Pass batch of preprocessed states to policy network.
Calculate loss between output Q-values and target Q-values.
Requires a pass to the target network for the next state
Gradient descent updates weights in the policy network to minimize loss.
After x time steps, weights in the target network are updated to the weights in the policy network.
example :

initial state of the screen

![initial state](https://user-images.githubusercontent.com/68875720/105173916-0375ce80-5b22-11eb-95c3-561c1599259b.jpg)


input state

![input state](https://user-images.githubusercontent.com/68875720/105174018-2f914f80-5b22-11eb-8604-083e9349cd3d.jpg)


training state

![training state](https://user-images.githubusercontent.com/68875720/105174135-66676580-5b22-11eb-8197-b1966a61674c.jpg)

