# Deep Learning

## Problem Type

| Sr. No. | Type                                   | Description                                                           |
| ------- | -------------------------------------- | --------------------------------------------------------------------- |
| 1       | Binary classification                  | each input sample should be categorized into two exclusive categories |
| 2       | Single-label Multiclass classification | each input sample should be categorized into more than two categories |
| 3       | Multi-label Multiclass classification  | each input sample can be assigned multiple labels                     |
| 4       | Scalar regression                      | target is a continuous scalar value                                   |
| 5       | Vector regression                      | target is a set of continuous values                                  |

## Activation

| Sr. No. | Activation | Description                                                                           |
| ------- | ---------- | ------------------------------------------------------------------------------------- |
| 1       | relu       | returns `max(x, 0)` for input x                                                       |
| 2       | softmax    | converts a vector of values to a probability distribution (Multiclass classification) |
| 3       | sigmoid    | 2-element Softmax (Binary classification)                                             |
| 4       | tanh       | similar to sigmoid (Binary classification)                                            |

## Optimizer

| Sr. No. | Optimizer | Description                                                                                  |
| ------- | --------- | -------------------------------------------------------------------------------------------- |
| 1       | rmsprop   | Maintain a moving average of the square of gradients, Divide the gradient by root of average |
| 2       | adam      | SGD method that is based on adaptive estimation of first-order and second-order moments.     |

## Loss Function

| Sr. No. | Loss Function                   | Description                          |
| ------- | ------------------------------- | ------------------------------------ |
| 1       | sparse_categorical_crossentropy | two or more label classes (integers) |
| 2       | binary_crossentropy             | Binary classification                |
| 3       | categorical_crossentropy        | two or more label classes            |
| 4       | mean_squared_error / mse        | regression                           |

## Matrics

| Sr. No. | Matrics  | Description                                                              |
| ------- | -------- | ------------------------------------------------------------------------ |
| 1       | accuracy | Calculates how often predictions equal labels                            |
| 2       | mae      | Absolute value ofthe difference between the predictions and the targets. |
| 3       | mse      | Square value of the difference between the predictions and the targets.  |
| 3       | ROC AUC  | area under a receiver operating characteristic (ROC)                     |
