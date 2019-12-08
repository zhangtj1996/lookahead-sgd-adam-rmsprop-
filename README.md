# lookahead-sgd-adam-rmsprop-
This repo gives some experimental results of the performance of lookahead optimizer and several well known stochastic algorithms (SGD, RMSProp, Adam). 

## Tasks
- Convex: Linear regression, logistic regression.
- Noncovex: Train an MLP.

## Data sets
- MNIST handwritten digits [http://yann.lecun.com/exdb/mnist/] (I picked out digits 7 and 8 for binary logistic regression)
- Residential Building Data Set [https://archive.ics.uci.edu/ml/datasets/Residential+Building+Data+Set]

## Requirement
- Mxnet https://mxnet.apache.org/
- Python 3.7

## Note
For logistic regression experment, the code for optimizers is not encapsulated, written according to the pseudo code provide in the reference below.
For the other experiments, I used the Mxnet framework, thanks to the implement in the repo https://github.com/wkcn/LookaheadOptimizer-mx. I modified the code optimizer.py according to the closed issue and fixed the bug.

## Reference 
Lookahead Optimizer: k steps forward, 1 step back https://arxiv.org/pdf/1907.08610.pdf
Adam: A Method for Stochastic Optimization https://arxiv.org/abs/1412.6980

