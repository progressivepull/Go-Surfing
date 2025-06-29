# Go-Surfing

* [Go Surfing](app.ipynb) - The “Go Surfing” neural network uses input features (waves, crowds, sharks), passes them through weighted layers with biases, applies the sigmoid function, and outputs a probability. If the output is above 0.5, the decision is to go surfing!

**1. Neural Networks and Their Layers**      
Neural networks are composed of layers of nodes (or artificial neurons). These layers include:     
* Input Layer: Takes in data.
* Hidden Layers: Process and transform data.
* Output Layer: Provides the final result.
  
These networks mimic the functioning of the human brain, enabling computers to recognize patterns and solve problems in AI and deep learning.
Technically, these should be referred to as **artificial neural networks (ANNs)** to differentiate them from natural neural networks in our brains.
Think of each artificial neuron as a standalone **linear regression model!**


**2. Nodes and Linear Regression**         
Each neuron performs a function similar to linear regression, which predicts future outcomes based on data. A single node is made up of:
* Input data.
* Weights (indicating the importance of each input).
* A bias (or threshold).
* An output.
  
Connections between nodes pass data through a structure called a **feed-forward network,** where data flows layer by layer.

**3. A Practical Example: Should We Go Surfing?**            
Let’s consider a decision-making node. The output,**Y-hat,** represents whether or not we should go surfing:

* **Input Variables:** X₁ for good waves (1 = yes, 0 = no), X₂ crowded beaches (1 = yes, 0 = no), and X₃ for a shark-free zone (1 = yes, 0 = no).     
* **Weights:** W₁ = 5 (good waves matter most), W₂ = 2 (less crowded lineup is less crucial), W₃ = 4 (avoiding sharks is highly important).     
* **Bias/Threshold:** -3.      
  
Plugging into the formula: **Y-hat = (X₁ × W₁) + (X₂ × W₂) + (X₃ × W₃) - Bias.**       
Assume X₁ = 1, X₂ = 0, X₃ = 1: **Y-hat = (1 × 5) + (0 × 2) + (1 × 4) - 3 = 6.**     
Since 6 > 0, the output is 1: **We’re going surfing!**    
Adjusting weights or the threshold can lead to different outcomes.          

**4. The Importance of Training Data**       
Neural networks rely on **training data** to improve their accuracy. Using **supervised learning** on labeled datasets, the model learns to minimize errors by:        
* Calculating errors through a **cost function**.      
* Adjusting weights and biases using a process called **gradient descent,** which optimizes the model to predict more accurately. **
