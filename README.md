Assignment-3: Growing Neural Network Training

![](Aspose.Words.384d325e-24fd-4f37-be07-9c20386a4f39.001.png)

ELL784: Introduction To Machine Learning

Submitted By

Bitthal Bhai Patel (2023EET2184)

Submitted To Prof. Jayadeval

**Contents**

[**1 Problem statement](#_page2_x70.87_y83.82) **1 [2 Procedure](#_page2_x70.87_y328.39) 1**

1. [DataSet ](#_page2_x70.87_y358.78). . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 1
1. [Training the individual nodes while using a standard activation function . . . ](#_page3_x70.87_y83.82). . . . . . . 2
1. [Avoiding Overfitting ](#_page3_x70.87_y233.11). . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
1. [Plotting Graph . ](#_page3_x70.87_y333.98). . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2

**IIT Delhi Software Fundamentals![](Aspose.Words.384d325e-24fd-4f37-be07-9c20386a4f39.002.png)**

<a name="_page2_x70.87_y83.82"></a>**1** | **Problem statement**

Consider your dataset that you built for Assignment 2. Use the same dataset to build a tree type growing neural network. At each node, learn a small neural network that tries to classify samples correctly, and child nodes are added to correct for misclassified samples. Explain how you will train the individual nodes while using a standard activation function, and then use the trained network as a node in a growing structure. Plot the loss function values and accuracies for training, validation, and test subsets, as the network is grown. Deduce a scheme to terminate growth to avoid overfitting. Please explain your approach and any assumptions in detail. Any missing detail may lead to hurdles in a fair evaluation. Use well designed figures to explain your approach and the growing network.

<a name="_page2_x70.87_y328.39"></a>**2** | **Procedure**

1. |<a name="_page2_x70.87_y358.78"></a> **DataSet**
- Using the DataSet used in Assignment-2

![](Aspose.Words.384d325e-24fd-4f37-be07-9c20386a4f39.003.png)

Figure 1:Neural Network![ref1]

2. |<a name="_page3_x70.87_y83.82"></a> **Training the individual nodes while using a standard activation function**
- Using TensorFlow added one neuron at a time.
- Also created child node.
- At last combined all neurons and give to output layer.
- used RMSprop optimizer.
3. |<a name="_page3_x70.87_y233.11"></a> **Avoiding Overfitting**
- Used Tensor Flow Regularization (L2) to avoid overfitting setting its value “0.01”.
- Applied to childs, hidden neuron (4,5) and at combined layer.
4. |<a name="_page3_x70.87_y333.98"></a> **Plotting Graph**
- Plotting the training, validation, and test loss values across epochs.

![](Aspose.Words.384d325e-24fd-4f37-be07-9c20386a4f39.005.png)

Figure 2:Loss graph across Epochs without Regularization![ref1]

![](Aspose.Words.384d325e-24fd-4f37-be07-9c20386a4f39.006.png)

Figure 3:Loss graph across Epochs with Regularization![ref1]
Page 3

[ref1]: Aspose.Words.384d325e-24fd-4f37-be07-9c20386a4f39.004.png
