For this experiment we used Kaggle’s SMS Spam Detection Dataset to build a spam/not-spam classifier with Flair. The dataset is suitable for learning as it only contains 5572 lines and it is small enough to train a model in a few minutes on a CPU.

![Capture](https://github.com/Achraf-99/myProjects/assets/115900714/4bf07c74-f849-4a5e-b5a5-876fc5981976)

We removed some duplicates from our dataset, shuffled it (randomise rows) and split the data into train, dev and test sets using the 80/10/10 split.

Next is the block of code that trains the model which produces 'final-model.pt' and 'best-model.pt' files which represent our stored trained model.

We can now use the exported model to generate predictions by running the 'predict' method of the classifier and see that our model has assured us 99% that the sentence is not a spam.

In our case we used the default hyper parameters for the sake of simplicity. With mostly default parameters our Flair model achieved an f1-score of  0.9884 after 10 epochs.

Note: Better to have the notebook open and follow along.
