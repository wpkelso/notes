#machine_learning 

### Overfitting vs Underfitting
- Overfitting: "learning the noise"; relation between data and curve is too close, and will not work with another data set, i.e. the model cannot be generalized
- Underfitting: assumption of the order of the model is too low, and won't fit any data well.

Ultimately we can't know the exact order of the underlying curve, so we'll have to guess a couple different orders and find the one that gives us the least error (related: [[Mean Squared Error]])

### Types of Error
- Variance Error: Related to training set; Will be high when slight changes in the changing set can increase the error
- Bias Error: Related to approximation; High when the underlying distribution is more complicated than the model 