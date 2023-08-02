# CUSTOM-CALLBACKS-KERAS

The objective is to write own callback function, that has to print the micro F1 score and AUC score after each epoch.Do not use tf.keras.metrics for calculating AUC and F1 score.

Save model at every epoch if validation accuracy is improved from previous epoch.

Use decay learning based on below conditions

      Cond1. If your validation accuracy at that epoch is less than previous epoch accuracy, you have to decrese the
             learning rate by 10%. 
      Cond2. For every 3rd epoch, decay your learning rate by 5%.

Use tensorboard for every model and analyse your scalar plots and histograms
