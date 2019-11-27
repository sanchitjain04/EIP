
# 20 Epochs:



Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.002.
60000/60000 [==============================] - 29s 488us/step - loss: 0.1046 - acc: 0.9526 - val_loss: 0.0216 - val_acc: 0.9940
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0015163002.
60000/60000 [==============================] - 22s 363us/step - loss: 0.1034 - acc: 0.9536 - val_loss: 0.0282 - val_acc: 0.9930
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0012210012.
60000/60000 [==============================] - 22s 364us/step - loss: 0.0973 - acc: 0.9548 - val_loss: 0.0225 - val_acc: 0.9939
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0010219724.
60000/60000 [==============================] - 22s 366us/step - loss: 0.0950 - acc: 0.9572 - val_loss: 0.0208 - val_acc: 0.9940
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0008787346.
60000/60000 [==============================] - 22s 364us/step - loss: 0.0953 - acc: 0.9561 - val_loss: 0.0258 - val_acc: 0.9934
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0007707129.
60000/60000 [==============================] - 22s 363us/step - loss: 0.0932 - acc: 0.9565 - val_loss: 0.0202 - val_acc: 0.9944
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0006863418.
60000/60000 [==============================] - 22s 368us/step - loss: 0.0938 - acc: 0.9560 - val_loss: 0.0217 - val_acc: 0.9940
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0006186205.
60000/60000 [==============================] - 22s 365us/step - loss: 0.0933 - acc: 0.9563 - val_loss: 0.0216 - val_acc: 0.9945
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0005630631.
60000/60000 [==============================] - 22s 363us/step - loss: 0.0882 - acc: 0.9586 - val_loss: 0.0230 - val_acc: 0.9946
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0005166624.
60000/60000 [==============================] - 22s 363us/step - loss: 0.0887 - acc: 0.9575 - val_loss: 0.0225 - val_acc: 0.9940
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.000477327.
60000/60000 [==============================] - 22s 363us/step - loss: 0.0874 - acc: 0.9589 - val_loss: 0.0216 - val_acc: 0.9946
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.0004435573.
60000/60000 [==============================] - 22s 370us/step - loss: 0.0876 - acc: 0.9592 - val_loss: 0.0220 - val_acc: 0.9946
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0004142502.
60000/60000 [==============================] - 22s 365us/step - loss: 0.0894 - acc: 0.9572 - val_loss: 0.0212 - val_acc: 0.9946
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0003885759.
60000/60000 [==============================] - 22s 363us/step - loss: 0.0877 - acc: 0.9577 - val_loss: 0.0201 - val_acc: 0.9949
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0003658983.
60000/60000 [==============================] - 22s 364us/step - loss: 0.0889 - acc: 0.9570 - val_loss: 0.0192 - val_acc: 0.9947
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0003457217.
60000/60000 [==============================] - 22s 363us/step - loss: 0.0886 - acc: 0.9562 - val_loss: 0.0200 - val_acc: 0.9946
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000327654.
60000/60000 [==============================] - 22s 364us/step - loss: 0.0870 - acc: 0.9576 - val_loss: 0.0194 - val_acc: 0.9947
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.000311381.
60000/60000 [==============================] - 22s 364us/step - loss: 0.0859 - acc: 0.9588 - val_loss: 0.0207 - val_acc: 0.9949
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0002966479.
60000/60000 [==============================] - 22s 365us/step - loss: 0.0870 - acc: 0.9575 - val_loss: 0.0201 - val_acc: 0.9950
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000283246.
60000/60000 [==============================] - 22s 364us/step - loss: 0.0868 - acc: 0.9577 - val_loss: 0.0207 - val_acc: 0.9953
<keras.callbacks.History at 0x7febcf5397b8>



# result of model.evaluate:
[0.020677942662581335, 0.9953]


## Strategy:
Kept the first 2 conv size as 16, learning rate as 0.2 and batch size as 64
