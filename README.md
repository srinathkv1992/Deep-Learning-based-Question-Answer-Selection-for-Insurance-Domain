# Deep Learning based Question Answer Selection for Insurance Domain
The approach used is CNN on top of an Bi directional LSTM framework.
The purpose of the project is for a question select the most appropriate answer for an answer pool.

Objective: For a question Q we select an answer A From a existing answer pool {a1, a2..aN}

DataSet: The data set used is  Insurance QA which is available on the following URL: https://github.com/shuzi/insuranceQA

Framework:
There are two frameworks used:
The basic framework  is a bi-directional LSTM framework.The question and answers are passed seperately to the LSTM seperately.
The output vectors from LSTM are then passed for max-pooling.
In the final step, Cosine similarity is used to find similarity between the question and answer vector.

![BASIC Bi-LSTM FRAMEWORK](https://github.com/srinathkv1992/Deep-Learning-based-Question-Answer-Selection-for-Insurance-Domain/blob/master/LSTM.PNG)

The advanced framework used is a Convolutional Neural Network on top of a Bi-directional LSTM.
The output vectors from LSTM and CNN are then passed for max-pooling.
In the final step, Cosine similarity is used to find similarity between the question and answer vector.






