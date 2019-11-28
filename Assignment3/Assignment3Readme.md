# Validation accuracy 

the validation accuracy is 79

# Model Defination

model = Sequential()
model.add(SeparableConv2D(48, kernel_size=(3, 3), activation='relu', input_shape=(32, 32, 3))) # N_out=23, RF=1

model.add(SeparableConv2D(48, kernel_size=(3, 3), activation='relu')) # N_out=23, RF=5
model.add(BatchNormalization())
model.add(Dropout(0.1))

model.add(SeparableConv2D(96, kernel_size=(3, 3), activation='relu')) # N_out=42, RF=7
model.add(BatchNormalization())
model.add(Dropout(0.1))

model.add(SeparableConv2D(96, kernel_size=(3, 3), activation='relu')) # N_out=42, RF=9
model.add(BatchNormalization())
model.add(Dropout(0.1))

model.add(SeparableConv2D(96, kernel_size=(3, 3), activation='relu')) # N_out=42, RF=11
model.add(BatchNormalization())
model.add(Dropout(0.1))

model.add(MaxPooling2D(pool_size=(2, 2))) # N_out=2, RF=13

model.add(SeparableConv2D(96, kernel_size=(3, 3), activation='relu')) # N_out=42, RF=15
model.add(BatchNormalization())
model.add(Dropout(0.1))


model.add(SeparableConv2D(128, kernel_size=(3, 3), activation='relu')) # N_out=64, RF=17
model.add(BatchNormalization())
model.add(Dropout(0.1))


model.add(SeparableConv2D(128, kernel_size=(3, 3), activation='relu')) # N_out=64, RF=19
model.add(BatchNormalization())
model.add(Dropout(0.1))

model.add(SeparableConv2D(128, kernel_size=(3, 3), activation='relu')) # N_out=64, RF=19
model.add(BatchNormalization())
model.add(Dropout(0.1))

model.add(SeparableConv2D(10, kernel_size=(3, 3), activation='relu')) # N_out=64, RF=19
model.add(BatchNormalization())
model.add(Dropout(0.1))

model.add(Flatten())
model.add(Activation('softmax'))

# Epoch Logs
Epoch 1/50
390/390 [==============================] - 67s 171ms/step - loss: 1.8189 - acc: 0.3552 - val_loss: 1.6985 - val_acc: 0.4139
Epoch 2/50
390/390 [==============================] - 37s 94ms/step - loss: 1.4154 - acc: 0.5090 - val_loss: 1.6981 - val_acc: 0.4169
Epoch 3/50
390/390 [==============================] - 37s 94ms/step - loss: 1.2582 - acc: 0.5665 - val_loss: 1.2454 - val_acc: 0.5736
Epoch 4/50
390/390 [==============================] - 37s 95ms/step - loss: 1.1506 - acc: 0.6028 - val_loss: 1.1090 - val_acc: 0.6158
Epoch 5/50
390/390 [==============================] - 36s 94ms/step - loss: 1.0651 - acc: 0.6324 - val_loss: 1.0806 - val_acc: 0.6314
Epoch 6/50
390/390 [==============================] - 36s 93ms/step - loss: 1.0060 - acc: 0.6522 - val_loss: 0.9765 - val_acc: 0.6702
Epoch 7/50
390/390 [==============================] - 36s 93ms/step - loss: 0.9462 - acc: 0.6739 - val_loss: 0.8725 - val_acc: 0.7059
Epoch 8/50
390/390 [==============================] - 36s 93ms/step - loss: 0.9017 - acc: 0.6892 - val_loss: 0.8812 - val_acc: 0.7001
Epoch 9/50
390/390 [==============================] - 36s 94ms/step - loss: 0.8634 - acc: 0.7017 - val_loss: 0.8261 - val_acc: 0.7212
Epoch 10/50
390/390 [==============================] - 37s 94ms/step - loss: 0.8272 - acc: 0.7123 - val_loss: 0.8117 - val_acc: 0.7275
Epoch 11/50
390/390 [==============================] - 36s 93ms/step - loss: 0.7974 - acc: 0.7227 - val_loss: 0.8582 - val_acc: 0.7201
Epoch 12/50
390/390 [==============================] - 36s 93ms/step - loss: 0.7827 - acc: 0.7256 - val_loss: 0.8336 - val_acc: 0.7238
Epoch 13/50
390/390 [==============================] - 36s 92ms/step - loss: 0.7515 - acc: 0.7384 - val_loss: 0.8363 - val_acc: 0.7209
Epoch 14/50
390/390 [==============================] - 36s 93ms/step - loss: 0.7293 - acc: 0.7451 - val_loss: 0.7846 - val_acc: 0.7426
Epoch 15/50
390/390 [==============================] - 36s 93ms/step - loss: 0.7095 - acc: 0.7524 - val_loss: 0.7489 - val_acc: 0.7562
Epoch 16/50
390/390 [==============================] - 36s 92ms/step - loss: 0.6878 - acc: 0.7592 - val_loss: 0.7949 - val_acc: 0.7387
Epoch 17/50
390/390 [==============================] - 36s 93ms/step - loss: 0.6652 - acc: 0.7678 - val_loss: 0.7748 - val_acc: 0.7448
Epoch 18/50
390/390 [==============================] - 36s 92ms/step - loss: 0.6505 - acc: 0.7711 - val_loss: 0.7211 - val_acc: 0.7666
Epoch 19/50
390/390 [==============================] - 36s 93ms/step - loss: 0.6346 - acc: 0.7762 - val_loss: 0.7296 - val_acc: 0.7626
Epoch 20/50
390/390 [==============================] - 36s 93ms/step - loss: 0.6236 - acc: 0.7788 - val_loss: 0.7104 - val_acc: 0.7697
Epoch 21/50
390/390 [==============================] - 36s 92ms/step - loss: 0.6080 - acc: 0.7844 - val_loss: 0.7003 - val_acc: 0.7706
Epoch 22/50
390/390 [==============================] - 36s 92ms/step - loss: 0.5955 - acc: 0.7891 - val_loss: 0.7365 - val_acc: 0.7610
Epoch 23/50
390/390 [==============================] - 36s 92ms/step - loss: 0.5782 - acc: 0.7949 - val_loss: 0.7761 - val_acc: 0.7460
Epoch 24/50
390/390 [==============================] - 37s 94ms/step - loss: 0.5620 - acc: 0.8026 - val_loss: 0.7416 - val_acc: 0.7609
Epoch 25/50
390/390 [==============================] - 36s 93ms/step - loss: 0.5591 - acc: 0.8023 - val_loss: 0.7588 - val_acc: 0.7540
Epoch 26/50
390/390 [==============================] - 36s 93ms/step - loss: 0.5507 - acc: 0.8046 - val_loss: 0.7009 - val_acc: 0.7715
Epoch 27/50
390/390 [==============================] - 37s 94ms/step - loss: 0.5409 - acc: 0.8087 - val_loss: 0.7043 - val_acc: 0.7721
Epoch 28/50
390/390 [==============================] - 36s 93ms/step - loss: 0.5285 - acc: 0.8115 - val_loss: 0.6944 - val_acc: 0.7808
Epoch 29/50
390/390 [==============================] - 37s 94ms/step - loss: 0.5227 - acc: 0.8133 - val_loss: 0.7358 - val_acc: 0.7652
Epoch 30/50
390/390 [==============================] - 36s 93ms/step - loss: 0.5084 - acc: 0.8197 - val_loss: 0.7313 - val_acc: 0.7623
Epoch 31/50
390/390 [==============================] - 36s 92ms/step - loss: 0.5066 - acc: 0.8202 - val_loss: 0.7763 - val_acc: 0.7541
Epoch 32/50
390/390 [==============================] - 37s 94ms/step - loss: 0.4970 - acc: 0.8224 - val_loss: 0.6769 - val_acc: 0.7896
Epoch 33/50
390/390 [==============================] - 36s 92ms/step - loss: 0.4937 - acc: 0.8235 - val_loss: 0.7737 - val_acc: 0.7551
Epoch 34/50
390/390 [==============================] - 36s 93ms/step - loss: 0.4793 - acc: 0.8295 - val_loss: 0.7053 - val_acc: 0.7774
Epoch 35/50
390/390 [==============================] - 36s 93ms/step - loss: 0.4751 - acc: 0.8307 - val_loss: 0.7646 - val_acc: 0.7618
Epoch 36/50
390/390 [==============================] - 36s 93ms/step - loss: 0.4640 - acc: 0.8333 - val_loss: 0.7323 - val_acc: 0.7724
Epoch 37/50
390/390 [==============================] - 36s 92ms/step - loss: 0.4664 - acc: 0.8337 - val_loss: 0.7855 - val_acc: 0.7663
Epoch 38/50
390/390 [==============================] - 36s 92ms/step - loss: 0.4520 - acc: 0.8384 - val_loss: 0.7339 - val_acc: 0.7750
Epoch 39/50
390/390 [==============================] - 36s 93ms/step - loss: 0.4516 - acc: 0.8372 - val_loss: 0.7321 - val_acc: 0.7756
Epoch 40/50
390/390 [==============================] - 36s 92ms/step - loss: 0.4392 - acc: 0.8431 - val_loss: 0.7176 - val_acc: 0.7799
Epoch 41/50
390/390 [==============================] - 36s 93ms/step - loss: 0.4406 - acc: 0.8405 - val_loss: 0.8083 - val_acc: 0.7616
Epoch 42/50
390/390 [==============================] - 36s 93ms/step - loss: 0.4342 - acc: 0.8439 - val_loss: 0.7722 - val_acc: 0.7702
Epoch 43/50
390/390 [==============================] - 36s 92ms/step - loss: 0.4242 - acc: 0.8465 - val_loss: 0.7118 - val_acc: 0.7880
Epoch 44/50
390/390 [==============================] - 36s 92ms/step - loss: 0.4266 - acc: 0.8460 - val_loss: 0.6962 - val_acc: 0.7879
Epoch 45/50
390/390 [==============================] - 36s 93ms/step - loss: 0.4183 - acc: 0.8474 - val_loss: 0.7060 - val_acc: 0.7881
Epoch 46/50
390/390 [==============================] - 36s 92ms/step - loss: 0.4176 - acc: 0.8490 - val_loss: 0.7012 - val_acc: 0.7840
Epoch 47/50
390/390 [==============================] - 36s 92ms/step - loss: 0.4161 - acc: 0.8484 - val_loss: 0.6845 - val_acc: 0.7877
Epoch 48/50
390/390 [==============================] - 36s 93ms/step - loss: 0.4065 - acc: 0.8513 - val_loss: 0.7121 - val_acc: 0.7943
Epoch 49/50
390/390 [==============================] - 37s 94ms/step - loss: 0.4020 - acc: 0.8540 - val_loss: 0.6981 - val_acc: 0.7911
Epoch 50/50
390/390 [==============================] - 36s 94ms/step - loss: 0.3973 - acc: 0.8559 - val_loss: 0.7184 - val_acc: 0.7875
Model took 1844.13 seconds to train
