# Dementia-MRI-Detection-
CNN architecture based Dementia detection model, achieving a accuracy of 97% in 16 epochs.

 Total params: 8,010,180 (30.56 MB)
 Trainable params: 8,002,564 (30.53 MB)
 Non-trainable params: 7,616 (29.75 KB)




Model Summary -



┃ Layer (type)                    ┃ Output Shape           ┃       Param # ┃

│ conv2d (Conv2D)                 │ (None, 248, 248, 32)   │           896 │

│ batch_normalization             │ (None, 248, 248, 32)   │           128 │
│ (BatchNormalization)            │                        │               │

│ max_pooling2d (MaxPooling2D)    │ (None, 124, 124, 32)   │             0 │

│ conv2d_1 (Conv2D)               │ (None, 122, 122, 64)   │        18,496 │

│ batch_normalization_1           │ (None, 122, 122, 64)   │           256 │
│ (BatchNormalization)            │                        │               │

│ max_pooling2d_1 (MaxPooling2D)  │ (None, 61, 61, 64)     │             0 │

│ conv2d_2 (Conv2D)               │ (None, 59, 59, 128)    │        73,856 │

│ batch_normalization_2           │ (None, 59, 59, 128)    │           512 │
│ (BatchNormalization)            │                        │               │

│ max_pooling2d_2 (MaxPooling2D)  │ (None, 29, 29, 128)    │             0 │

│ conv2d_3 (Conv2D)               │ (None, 27, 27, 256)    │       295,168 │

│ batch_normalization_3           │ (None, 27, 27, 256)    │         1,024 │
│ (BatchNormalization)            │                        │               │

│ max_pooling2d_3 (MaxPooling2D)  │ (None, 13, 13, 256)    │             0 │

│ conv2d_4 (Conv2D)               │ (None, 11, 11, 512)    │     1,180,160 │

│ batch_normalization_4           │ (None, 11, 11, 512)    │         2,048 │
│ (BatchNormalization)            │                        │               │

│ max_pooling2d_4 (MaxPooling2D)  │ (None, 5, 5, 512)      │             0 │

│ conv2d_5 (Conv2D)               │ (None, 3, 3, 1024)     │     4,719,616 │

│ batch_normalization_5           │ (None, 3, 3, 1024)     │         4,096 │
│ (BatchNormalization)            │                        │               │

│ max_pooling2d_5 (MaxPooling2D)  │ (None, 1, 1, 1024)     │             0 │

│ flatten (Flatten)               │ (None, 1024)           │             0 │

│ dense (Dense)                   │ (None, 1024)           │     1,049,600 │

│ batch_normalization_6           │ (None, 1024)           │         4,096 │
│ (BatchNormalization)            │                        │               │

│ dropout (Dropout)               │ (None, 1024)           │             0 │

│ dense_1 (Dense)                 │ (None, 512)            │       524,800 │

│ batch_normalization_7           │ (None, 512)            │         2,048 │
│ (BatchNormalization)            │                        │               │

│ dense_2 (Dense)                 │ (None, 256)            │       131,328 │

│ batch_normalization_8           │ (None, 256)            │         1,024 │
│ (BatchNormalization)            │                        │               │

│ dropout_1 (Dropout)             │ (None, 256)            │             0 │

│ dense_3 (Dense)                 │ (None, 4)              │         1,028 │

