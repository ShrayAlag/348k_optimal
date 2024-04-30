# CS 348K Stanford University Project Proposal
## Fast Inference Machine Learning Cost Model for General C++ Programs as a Basis for Optimal Code Efficiency Pipelines
Ideated, Written, and Implemented by Shray Alag; alag@stanford.edu (SuNET: alag)

#### Summary: I am going to build an end to end demo system that can taken in a relatively simple, functional C++ program and will predict the expected runtime of the program quickly (at the moment thinking of < 1 second). I will demonstrate success through the cost model's training accuracy, the real-time performance of the cost model, and the efficiency of the cost model's execution. I will be creating thousands of simple randomly generated C++ programs (with variety of loops, arithmetic, etc), benchmark their runtimes, use the programs and their runtimes as a dataset, create a machine learning model based on program's features and features present in the program's abstract syntax tree, and optimize the model for fast inference. By the end of the project, I hope to have accomplished my extremely ambitious goal of making an accurate and efficient machine learning model for predicting simple general C++ program runtimes. By "simple," I mean one class, possibly one function code that interacts with (a) loops, (b) arithmetic, (c) reading from and writing to a file, and (d) interacting with basic data structures. I'm extremely dedicated & fascinated by this project as such a model would be paramount in exploring more efficient representations of general purpose C++ code.  

#### Inputs & Outputs: The inputs will be randomly generated "simple" (see definition above) C++ code segments, features about such programs, and their benchmarked times; the outputs will be predictions of the amount of time the segment would take to run, meaning the ML cost model task is a regression. This problem is particularly fascinating to me as, to my best knowledge, there has been no prior work in this field of estimating the run time of general purpose programs The major constraints are machine performance—


#### Task List:


##### Expected Deliverables and/or Evaluation


##### What do I need help with?
