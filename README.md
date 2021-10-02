# Random forest

So what if our descion tree model does not perform well . What are the solutions for better performance?
The answer is in the ensemble methods.

The random forest model can be considered as an ensemble of decision trees. The idea behind a random forest is to average multiple (deep) decision trees that individually suffer from high variance, to build a more robust model that has a better generalization performance and is less susceptible to overfitting. 

![image](https://user-images.githubusercontent.com/53411455/135700637-b62663b1-0dcf-46c9-a5ad-77d258357bd6.png)


# Data

This repository contains an application of the random forest model on Iris dataset

# Conclusion

By increasing the number of trees (from 5 to 100 trees) in our model, we got 97% accuracy better than the linear models or a single decision tree, without tuning any parameters. We could adjust the max_features setting, or apply pre-pruning as we did for the single decision tree. However, often the default parameters of the random forest already work quite well.
Similarly to the decision tree, the random forest provides feature importances, which are computed by aggregating the feature importances over the trees in the forest. Typically, the feature importances provided by the random forest are more reliable than the ones provided by a single tree.

