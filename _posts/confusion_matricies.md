## Confusion Matricies
A confusion matrix is an permformance measurment tool for machine leaning data classification with two or more classes. No matter how many classes, the classification it'self can be one of four things: a true positive (TP), a false positive (FP), a true negative (TN), or a false negative (FN). 

For example, say we were identifying frogs from images of frogs and not frogs. If I had an image of a frog and our model identified it as a frog, this would be a true positive. If I had a cat and the model identified this as not a frog, this would be a true negative. If I had an image of a cat and the model classified this as an image of a from, this would be a false positive. If I had an image of a frog and the model classified this as not a frog, this would be a false negative. 

For a two class model, such as frogs and not frogs, we represent this data in a confusion matrix as below. We aim to have maximum values on the diagonals and zeros off this diagonal. 

![image](https://github.com/CaitiePhillips/CaitiePhillips.github.io/assets/61171103/2a865b80-4e97-432b-b785-ccfe2f2b3afa)

Extending this to a model with more classes, we would have something similar to below. Here, the diagonal elements are the correct classifications rather than true positives or negatives and the off diagonal elements are misclassifications rather than false negatives of positives (these terms work best in the two class example). 

![image](https://github.com/CaitiePhillips/CaitiePhillips.github.io/assets/61171103/06e31848-2412-420c-9f36-ffbfcfd64703)

We can use confidence matricies to calculate sensivity, specificity and accuracy; 
<img width="839" alt="image" src="https://github.com/CaitiePhillips/CaitiePhillips.github.io/assets/61171103/68fe7dcb-b481-4ca7-8153-9b04fcc386db">

Confusion matricies can be implimented to measure the performance of our model in the jupiter notebook with fastai's ClassificationInterpretation class and the plot_confusion_matrix method. 
