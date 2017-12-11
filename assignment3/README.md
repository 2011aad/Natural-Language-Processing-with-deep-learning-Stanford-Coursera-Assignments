# Some notification for assignment 3

In the 3rd part question (d) of Assignment 3, when learning the latching behavior of the rnn model, it should be noticed that we are using the @state of the rnn cell instead of the @output. Because as described in question (a), we compare the internal state of the cell with the actual sequence ie. @y.

In rnn model, the @state of the cell is for internal computation and the @output is for calculating the @preds used in softmax_loss. In vanilla rnn or gru model, the @state and the @output are the same. However, it is not true for lstm model. It is important to understand this difference.
