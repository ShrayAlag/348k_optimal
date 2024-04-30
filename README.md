# CS 348K Stanford University Project Proposal
## Fast Inference Machine Learning Cost Model for General C++ Programs as a Basis for Optimal Code Efficiency Pipelines
Ideated, Written, and Implemented by Shray Alag; alag@stanford.edu (SuNET: alag)

**Summary:** I am going to build an end to end demo system that can taken in a relatively simple, functional C++ program and will predict the expected runtime of the program quickly (at the moment thinking of < 2 seconds). I will demonstrate success through the cost model's training accuracy, the real-time performance of the cost model, and the efficiency of the cost model's execution. I will be creating thousands of simple randomly generated C++ programs (with variety of loops, arithmetic, etc), benchmark their runtimes, use the programs and their runtimes as a dataset, create a machine learning model based on program's features and features present in the program's abstract syntax tree, and optimize the model for fast inference. By the end of the project, I hope to have accomplished my extremely ambitious goal of making an accurate and efficient machine learning model for predicting simple general C++ program runtimes. By "simple," I mean one class, possibly one function code that interacts with (a) loops, (b) arithmetic, (c) reading from and writing to a file, and (d) interacting with basic data structures. I'm extremely dedicated & fascinated by this project as such a model would be paramount in exploring more efficient representations of general purpose C++ code.  

**Inputs & Outputs:** The inputs will be randomly generated "simple" (see definition above) C++ code segments, features about such programs, and their benchmarked times; the outputs will be predictions of the amount of time the segment would take to run, meaning the ML cost model task is a regression. The most major constraint is human time as I'm doing this project by myself and a lot of the work to get this project to a high bar will take enourmous amounts of time. Some goals I are that the model should be have an average error rate of < 35%, and that the model should run in < 2 seconds. These are not hard cutoffs but aspirational objectives I hope to achieve.


**Task List:** Please refer to the previous two paragraphs for more detaisl aboutt the overall approach as it is flushed out there. 
Task List:
1. Research into normal grammar syntax for C++ programs, specifically for the features of (a) loops, (b) arithmetic, (c) reading from and writing to a file, and (d) interacting with basic data structures.
2. Create criteria for features to add in the random C++ programs.
3. Create random code generator for the features and for the random C++ programs.
4. Generate tens of thousands of random code snippets.
5. Research into compute power needed to run the various programs correctly.
6. Write code to compile the various programs and to benchmark only the correctly compiled programs.
7. Research into methods to extract features from AST representations.
8. Run the tens of thousands of code snippets.
9. Store all of the run data.
10. Divide data into training, test, validation
11. Create baseline Machine Learning Model (MLP, or simple neural network)
12. Create more advanced ML models (2-10 layers, etc)
13. Fine tune parameters
14. Optimize/Shrink model for performance
15. Evaluate and Test to receive results


**Expected Deliverables and/or Evaluation:** I am hoping for a demo of how a simple C++ program can be fed into the ML model and how the model can predict the runtime of the program in real time. I would like to show the runtime my model estimates and compare it with the real run time that I show the viewer live. To the best of my knowledge, I do not believe any project has made any significant tackle into estimating runtime costs for general purpose languages like C++. My main goal for this project therefore, considering that I am working alone on it and I have other classes which require some time, is to get the whole pipeline above working and working with a solid accuracy (hopefully less 35% error) and with quick performance (less than 2 seconds). Proving that a semi-accurate estimation of a general purpose coding language can be successful in 5 weeks is, to me, a huge success in it of itself; if I am able to do so with robust regression accuracy and with efficient performance would be incredible.

**What are the biggest risks?** The single biggest risk to me is that because I'm doing this project by myself, I won't have the aid of another pair of eyes if I get stuck on one of the tasks. Additionally, some other risks are if I am not able to create compilable, automatically generated random code and if the features I am able to extract from the program are too noisy/meaningless: if either of these things fail, it will be very hard for me to proceed with my project. Finally, if I am unable to get my machine learning model to work, perhaps because the features I am extracting are of variable length and size, I will be at a loss for how to proceed. I think the best approach if I am faced with any of these blockers is to pivot my idea or look for different means at bypassing the task (looking for different ways to extract meaningful signals, etc for instance).

**What do I need help with?** I am super excited and dedicated to this project; however, I haven't done most of the coding tasks—like automatically generating random code, creating code to extract features from code & ASTs, running thousands of programs in parallel or on a GPU—before. It would be very helpful to talk to Kayvon every so often to get his opinion on how to best move forward, particularly at blocking points. Further, I will likely need access to compute resources for running (and perhaps storing) thousands of code segments. 

I will be referencing the Halide autoscheduler paper, "Learning to Optimize Tensor Programs" (https://arxiv.org/pdf/1805.08166), and "TVM: An Automated End-to-End Optimizing Compiler for Deep Learning" (https://www.usenix.org/system/files/osdi18-chen.pdf) for inspiration and implementation guidance. 
