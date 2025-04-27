# Experimental-Analysis-on-Smart-Contract-Vulnerabilities-using-ML-DL-Models


This research uses CNN with Transformer architecture as presented in figure 1 to identify 
vulnerabilities in smart contracts. The smart contracts (.sol files) have components like SPDX 
License Identifier, Pragmas Version, Import statements, Contract declaration statements and 
other tokens like delimiters and punctuators which may hamper the processing of the Model, 
in order to overcome this shortcoming. The model analyzes sequences of tokenized 
representations until it reaches its token limit at 128 followed by dense embedding conversion. 
Transformers need additional positional encoding because they normally lose track of 
sequence information

The CNN-Transformer block contains three elements featuring a 1D convolutional layer that 
detects contextual token connections besides a max-pooling layer which shortens sequences 
while retaining critical information. Multi-head attention in transformers allows the system to 
discover distant correlations by evaluating dependencies among all tokens in their transformed 
representations[15]. Such feed-forward combination strengthens the model to detect complex 
relationships in data. The squeeze-and-excitation block enhances both model conduct along 
with representational capability by adjusting channel- wise feature responses. The essential 
token-level features go through global max pooling which results in a condensed 
 representation. Each dense layer adopts weighted values to form complex decision boundaries 
through non-linear activated functions during its execution of input features from previous 
layers. The refined inputs undergo softmax activation in the output layer to determine 
multiclass classifications using probabilistic distributions. Security analysis of smart contracts 
receives optimization from the CNN-transformer framework which integrates local feature 
extraction of CNN with transformer-dependent features from distant locations.

The dataset consists of over 3K real-world Ethereum smart contracts from various resources 
where inherited contracts were also included. These contracts were selected focusing on the 
four types of vulnerability, where we implement the pre- processing methods. The contracts 
have been previously audited and contain contracts with vulnerabilities expecting it to be a 
good test for the detection tools. 


The Figure 2 attached represents a scatter plot of the vulnerabilities in terms of the predicted 
probabilities for the different classes. Each class represent a type of vulnerability such as 
Delegate Call (DC), Integer Overflow (IO), Re-Entrency (RE), Timestamp Dependency (TD). 
Every dot corresponds to a particular sample selected from the test dataset; on the horizontal 
axis we have the true class labels; on the vertical axis, the model’s predicted probability for 
one. The process involves identifying samples belonging to each class and plotting the 
predicted probabilities (y_pred[:, class_idx]. This visualization emphasizes the spread and 
distribution of the dataset, highlighting the patterns and class specific variations. 
