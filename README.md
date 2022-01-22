# Data Privacy Project

### Description

Encrypt and Decrypt Files using Face Recognition.

### Usage

**Create Database**

Store a few images of the user in ./dataset/user folder

```
cd dataset
cd user
```

Store a few images of random people in ./dataset/unknown folder

```
cd ..
cd unknown
```

**Create Embeddings**
To create embeddings for the user, run the following command -

```
python face_detection.py
```

This will store the embeddings in the pickle folder

**Train Classification Model**
To train the SVM classification model, run the following command -

```
python model.py
```

**Encrypt and Decrypt Files**
To encrypt files -

```
python main.py -f [FILE PATH] -m encrypt
```

To decrypt files -

```
python main.py -f [FILE NAME] -m decrypt
```

The face of the user will be recognized using the webcam. If the user is matched, the file will be decrypted.
