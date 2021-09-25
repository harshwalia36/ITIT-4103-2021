# naivebayes_mnist
I implemented a Naive Bayes classifier form scratch and applied it on MNIST dataset.

The overall error is 18.51% (which is about 81.49% accuracy). The digits 0 and 1 tend to have minimal error rate compare to the other digits, this can be attributed to the fact that the digits 0 and 1 have low variabilities. Generally, people tend to write digits 0 and 1 in the right way.

Digits 4 & 5 have the high error rates, visualizing some of them show that they have high variations. Digit 4 is mostly misclassified has 9, some people tend to write 4 in a way that it looks like 9. Also, digit 2 is mostly misclassified as 8.

Digit 9 is mostly misclassified as either 4 or 8, likewise, digits 4 and 8 are also occasionally misclassified as 9.

Visualizing the 784 conditional probabilities per class (as 28 x 28 images) for a test sample with actual label 1 which is rightly classified:
![image](https://user-images.githubusercontent.com/43993467/134775705-07d65fcc-08fc-401e-bf56-9e3969d30036.png)

Visualizing the 784 conditional probabilities per class (as 28 x 28 images) for a test sample with actual label 4 which is wrongly classified as 9:
![image](https://user-images.githubusercontent.com/43993467/134775734-1dd4e016-261f-4346-bcd3-f85c47e36e0b.png)


Generally, Naive Bayes did poorly on the MNIST dataset, this could be attributed to the independent assumption which is likely not to be correct. Query time is faster compared to KNN, however, KNN provided better performance on the MNIST dataset. Naive Bayes doesn't perform well when there are repeated attributes or when attributes are not equally important, which are the case in the MNIST dataset.
