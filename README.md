# Kaggle-MNIST

## Introduction

MNIST ("Modified National Institute of Standards and Technology") is the de facto “hello world” dataset of computer vision. Since its release in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. As new machine learning techniques emerge, MNIST remains a reliable resource for researchers and learners alike.

Click [here][1] to read more on the Kaggle competition.

## Approach

Drawing inspiration from this [simple and helpful tutorial][3], I used the SVM classifier.

Tried my hand in data augmentation through [Keras' `ImageDataGenerator`][4], and create two models: One with augmentation, and one without, to see which fares better:

- Non-augmented scores 0.97100.

- Augmented scores 0.97200.

I referred a little to this [highly upvoted example][2] in Kaggle by Yassine Ghouzam. Thing is, I didn't apply much of anything that he did. For one, he uses CNN, and my attempts use SVM. Most of the stuff in his notebook just goes over my head.

## Files

`clf.joblib` and `clfa.joblib` are the models for my non-augmented and augmented approaches respectively.

`sample_submission.csv` is obtained from Kaggle; it tells us the format of submission.

Train and test data are located in the `\input` directory.

`a-beginner-s-approach-to-classification.ipynb` is the notebook that I referenced from mostly.

Last Updated 28 April 2020

[1]: https://www.kaggle.com/c/digit-recognizer/overview	"Kaggle: Digit Recognizer"
[2]:https://www.kaggle.com/yassineghouzam/introduction-to-cnn-keras-0-997-top-6#4.-Evaluate-the-model	"Introduction to CNN Keras - 0.997 (top 6%)"
[3]:https://www.kaggle.com/archaeocharlie/a-beginner-s-approach-to-classification/data	"A Beginner's Approach to Classification"
[4]: https://keras.io/preprocessing/image/

