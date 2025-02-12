# Optimizing-RUL-Prediction-with-LSTM

In this project, we built an LSTM-based deep learning model to predict the Remaining Useful Life (RUL) of aircraft engines using the CMAPSS dataset (FD001 subset). The dataset was preprocessed by normalizing sensor readings and generating RUL labels based on engine cycles. We then structured the data into sequences of 50 time steps to be fed into an LSTM model, which is well-suited for time-series forecasting tasks.

The model architecture consisted of two LSTM layers (100 and 50 units), dropout regularization (0.2), and a dense output layer. We trained the model for 20 epochs with the Mean Squared Error (MSE) loss function and the Adam optimizer. The training loss showed a steady decrease, indicating learning progress, while validation loss also improved significantly, dropping from 6409 to 839 over the epochs.

Key Performance Metrics:
Mean Absolute Error (MAE): 17.77
Root Mean Squared Error (RMSE): 28.97
These results suggest that the model is able to reasonably predict RUL, though there is still room for improvement. Possible enhancements could include hyperparameter tuning, deeper architectures, feature engineering, or additional data augmentation techniques.

The final visualization comparing true vs. predicted RUL indicates that while the model captures the general trend, it still has some variance in exact predictions. Overall, this study demonstrates the effectiveness of LSTMs in predictive maintenance tasks, showcasing their ability to handle complex sensor-based time-series data.
