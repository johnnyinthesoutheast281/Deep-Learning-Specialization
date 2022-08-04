# Single Number Evaluation Metric
When evaluating and tuning the hyperparameters of a model, it is better for us to use a single metric to evaluate the model performance rather than having too much evaluation metric i.e precision and recall. 

Suppose we are training a classification model to detect whether the patient is potentially has cancers or not. We train two classifier: the first classifier reached 95 percent in precision (of all the pictures that the classifier recognize a cat, what percentage is the classifier) and 90 percent in recall (of all the cat pictures, what percentage did the classifier got it right), the second classifier reached 99 percent in precision but only achieved 82 percent recall. Now it is confusing for us to determine which classifier performs better.

In order to choose, we will need to choose a metric that can generalize the problem. Suppose the problem is detecting cancers for the patient, we know that we dont want to detect the cancers patient as not having cancers, but we can sacrifice the percentage that the not-having-cancer patient as cancer, so we will focus on the recall metric rather than the precision metric. We want our classifier to not miss any having-cancer patient.

In the cat classification problem, we can use F1 Score to evaluate the performance of the classifiers. So, the first classifier will have 92.4 percent in F1 score and 89.7 percent in F1 Score for the second classifier. Now we can determine which classifier we should choose.  

# Satisficing and Optimizing Metric


# Train / Dev / Test Sets Distribution