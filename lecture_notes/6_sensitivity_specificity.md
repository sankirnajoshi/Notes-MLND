## Sensitivity and Specificity

---
Although similar, *sensitivity* and *specificity* are not the same as *precision* and *recall*. Here are the definitions:

In the cancer example, sensitivity and specificity are the following:

- Sensitivity: Of all the people **with** cancer, how many were correctly diagnosed?
- Specificity: Of all the people **without** cancer, how many were correctly diagnosed?

And precision and recall are the following:

- Recall: Of all the people who **have cancer**, how many did **we diagnose** as having cancer?
- Precision: Of all the people **we diagnosed** with cancer, how many actually had cancer?

From here we can see that Sensitivity is Recall, and the other two are not the same thing.

Trust me, we also have a hard time remembering which one is which, so here's a little trick. If you remember from Luis's Evaluation Metrics section, here is the confusion matrix:

<img src="images/confusion-matrix.png" width="600"/>

Now, sensitivity and specificity are the rows of this matrix. More specifically, if we label

- TP: (True Positives) Sick people that we **correctly** diagnosed as sick.
- TN: (True Negatives) Healthy people that we **correctly** diagnosed as healthy.
- FP: (False Positives) Healthy people that we **incorrectly** diagnosed as sick.
- FN: (False Negatives) Sick people that we **incorrectly** diagnosed as healthy.

then:

$$Sensitivity = \frac{TP}{TP + FN}$$

and

$$Specificity = \frac{TN}{TN + FP}$$


<img src="images/sensitivity-specificity.png" width="600"/>

Sensitivity and Specificity

And precision and recall are the top row and the left column of the matrix:

$$Recall = \frac{TP}{TP + FN}$$

and

$$Precision = \frac{TP}{TP + FP}$$

<img src="images/precision-recall.png" width="600"/>