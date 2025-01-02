# AI 筆記
## 1 | Machine Learning
### 1-1 | What is Machine Learning?
Computers learning via `data` and `experience` to predict events is machine learning.<br>
For instance:
- Speech Recognition
- Image Recognition
- Game Playing
- etc...

### 1-2 | Machine Learning v.s. Deep Learning
- Machine Learning: Analyzing input data to produce corresponding output, letting systems possess the ability to study by itself.
- Deep Learning: Mostly refers to deep artificial neural networks, allowing `human-like` decision, judgment and learning.

![Machine Learning v.s. Deep Learning](MLvsDL.png)

### 1-3 | Different Tasks of Machine Learning
- Regression: Constructing a function that outputs a scalar and fits the scenario.
- Classification: Constructing a function that outputs a class and fits the scenario.

### 1-4 | Types of Machine Learning
- Supervised Learning
    - Trait Detection using Labeled Data
    - Compare label with results to compute difference and act accordingly
    - **Advantage**: Higher precision
    - **Disadvantage**: Requires manual operation to label traits. Almost impossible when facing unknown fields. 
- Unsupervised Learning
    - No markings on any data
    - Machine automatically finds traits on data and classifies on its own
    - **Advantages**: Drastically reduces complex human work.
    - **Disadvantages**: Lower accuracy, could produce biased results, produce ineffective grouping results and unimportant traits could be overmagnified.
- Semi-supervised Learning
    - Markings on little data
    - Machine finds traits based on marked data and performs classification
    - Because recognition foundations are present, results are often more accurate than unsupervised learning.
- Reinforcement Learning
    - Doesn't provide the machine any data, has the machine learn based on interactions with the environment
    - Learns based on positive and negative feedbacks to obtain a higher reward
    - Predictions become more accurate over time, and the machine more efficiently performs the action to reach the target.

#### Diagram
```mermaid
graph TD
    A[Machine Learning] --> B[Supervised Learning]
    A --> C[Unsupervised Learning]
    A --> D[Reinforcement Learning]

    B --> E[Regression]
    B --> F[Classification]

    C --> G[Clustering]
    C --> H[Dimensionality Reduction]

    D --> I[Policy Optimization]
    D --> J[Value-Based Methods]
    D --> K[Model-Free Methods]
```
### 1-5 | 7 Steps of Machine Learning
1. Gathering data
2. Preparing data
3. Choosing a model
4. Training
5. Evaluation
6. Hyperparameter tuning
7. Prediction
### 1-6 | Model of Machine Learning
- SVM
- Decision Tree
- KNN
- Random Forest
- Gradient Boosting
- K-means
### 1-7 | Framework of Machine Learning
#### Overview
- Classify data into **training data** and **testing data**
- Train model
    1. Function with unknown
    2. Define loss from training data
    3. Optimization

```mermaid
graph TD
    A[How to Train Better]
    A --> B[Loss on Training Data]
    A --> F[Loss on Testing Data]
    B --> C[Large Loss]
    B --> D[Small Loss]
    F --> G[Large Loss]
    F --> H[Small Loss]
    
    C --> I[Optimization]
    D --> J[Model Bias]
    J --> K[Make Model More Complex]
    K --> L[Trade Off]
    L --> M[Split Training Data for Model Selection]

    G --> N[Overfitting]
    G --> O[Mismatch]
    N --> P[More Training Data]
    N --> Q[Data Augmentation]
    N --> R[Make Model Simpler]

    H --> S[Success]
```
#### Model Bias & Optimization
![Model Bias and Optimization Issue](ModelBiasAndOptimization.png)
#### Underfitting & Overfitting
- **Underfitting**: The model cannot accurately explain the relationship between pieces of data.
    - <u>Resolution</u>: Selected too few input traits. Make the model more complex.
- **Overfitting**: The model overexplains data.
    - <u>Resolution</u>: Increase training data, data agumentation, make model simpler
#### Bias-Complexity Trade-off
![Bias-Complexity Trade-off](Bias_Complexity_Tradeoff.png)
