This folder is used for clean to clean mapping verification using DNN.

And this clean to clean mapping is also a verification for the whole feature extraction, training, decoding and evaluation process

We train the model using the standard TIMIT training set and using the standard TIMIT test set as testing.

The final PESQ on the TIMIT test utterance can be as high as 4.4 (The PESQ value range is [0, +4.5], higher better)

Steps (keras with tensorflow backend):
step0: modify the config.py for your paths
step1: python prepare_fea.py
step3: python main_train_sednn_keras_v2.py
step4: python main_decode_sednn_keras.py
step5: ./pesq ref.wav enh.wav +16000

The trained DNN model on TIMTI training set which can bring the PESQ upto 4.4 on TIMIT test set: 
https://drive.google.com/file/d/1MtW2e1-9A5whiwJemc9VQnKTFV9L10bY/view

https://doc-0c-74-docs.googleusercontent.com/docs/securesc/oe2ljl52r1hfh6uepkcv7p0ueku5dma4/p0qcv3eeo56cnb54e89lcdp7ma7s2aa1/1543917600000/10772721672415841223/08628925364679730404/1MtW2e1-9A5whiwJemc9VQnKTFV9L10bY?e=download&nonce=cs9nmp4hmp4q4&user=08628925364679730404&hash=nitm4o0cqkll5jm02d88pdprsg78rrth

The training loss can be as low as "zero"!!!!
880564/880564 [==============================] - 39s - loss: 0.1572 - val_loss: 0.0854
Epoch 2/10000
880564/880564 [==============================] - 39s - loss: 0.0652 - val_loss: 0.0529
Epoch 3/10000
880564/880564 [==============================] - 36s - loss: 0.0439 - val_loss: 0.0398
Epoch 4/10000
880564/880564 [==============================] - 34s - loss: 0.0331 - val_loss: 0.0293
Epoch 5/10000
880564/880564 [==============================] - 34s - loss: 0.0265 - val_loss: 0.0255
Epoch 6/10000
880564/880564 [==============================] - 34s - loss: 0.0220 - val_loss: 0.0212
Epoch 7/10000
880564/880564 [==============================] - 33s - loss: 0.0187 - val_loss: 0.0179
Epoch 8/10000
880564/880564 [==============================] - 34s - loss: 0.0163 - val_loss: 0.0151
Epoch 9/10000
880564/880564 [==============================] - 33s - loss: 0.0142 - val_loss: 0.0128
Epoch 10/10000
880564/880564 [==============================] - 33s - loss: 0.0126 - val_loss: 0.0124
Epoch 11/10000
880564/880564 [==============================] - 33s - loss: 0.0113 - val_loss: 0.0107
Epoch 12/10000
880564/880564 [==============================] - 33s - loss: 0.0104 - val_loss: 0.0100
Epoch 13/10000
880564/880564 [==============================] - 34s - loss: 0.0094 - val_loss: 0.0093
Epoch 14/10000
880564/880564 [==============================] - 33s - loss: 0.0087 - val_loss: 0.0080
Epoch 15/10000
880564/880564 [==============================] - 34s - loss: 0.0080 - val_loss: 0.0077
Epoch 16/10000
880564/880564 [==============================] - 34s - loss: 0.0075 - val_loss: 0.0073
Epoch 17/10000
880564/880564 [==============================] - 34s - loss: 0.0068 - val_loss: 0.0068
Epoch 18/10000
880564/880564 [==============================] - 34s - loss: 0.0065 - val_loss: 0.0060
Epoch 19/10000
880564/880564 [==============================] - 34s - loss: 0.0059 - val_loss: 0.0059
Epoch 20/10000
880564/880564 [==============================] - 34s - loss: 0.0057 - val_loss: 0.0065
Epoch 21/10000
880564/880564 [==============================] - 34s - loss: 0.0053 - val_loss: 0.0050
Epoch 22/10000
880564/880564 [==============================] - 33s - loss: 0.0049 - val_loss: 0.0048
Epoch 23/10000
880564/880564 [==============================] - 34s - loss: 0.0047 - val_loss: 0.0045
Epoch 24/10000
880564/880564 [==============================] - 34s - loss: 0.0043 - val_loss: 0.0043
Epoch 25/10000
880564/880564 [==============================] - 33s - loss: 0.0043 - val_loss: 0.0039
Epoch 26/10000
880564/880564 [==============================] - 34s - loss: 0.0040 - val_loss: 0.0036
Epoch 27/10000
880564/880564 [==============================] - 38s - loss: 0.0037 - val_loss: 0.0034
Epoch 28/10000
880564/880564 [==============================] - 42s - loss: 0.0035 - val_loss: 0.0032
Epoch 29/10000
880564/880564 [==============================] - 42s - loss: 0.0033 - val_loss: 0.0035
Epoch 30/10000
880564/880564 [==============================] - 41s - loss: 0.0032 - val_loss: 0.0031
Epoch 31/10000
880564/880564 [==============================] - 33s - loss: 0.0031 - val_loss: 0.0048
......................................................
......................................................
