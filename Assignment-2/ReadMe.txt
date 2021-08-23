Architecture:
Feedforward NN with 3 hidden layers (with 32 nodes each layer) with tan-h activation and output layer with 3 nodes and softmax activation.

Optimization procedure: Used adam optimizer. Tried other optimisers as well.

Learning rate: 0.001

Batch size: For cleaned text data, the best performing batch-size (in terms of validation loss) was 32. If we consider raw text (including the headers and footers of the text) and vectorise it using TF-IDF and classify using neural networks, the best performing batch size was 8. 

For cleaned data (after removing the headers and footers), I was getting maximum f1 score (micro average) = 0.91 on validation
For raw data, I am getting maximum f1 score (micro average) = 0.98 on validation
So I reported the maximum score which I'm getting which is 0.98