# Deep-learning
This repository contains course assignments of Deep Learning in Eindhoven Univeristy of Technology.

# Contents
## Word Embedding
Build word embeddings using CBOW model and Skipgram model with a Keras implementation. Perform the analogy task by comparing the similarity between word embeddings. A sample analogy task likes: "a king is to a queen as a man is to a woman" ($e_{king} - e_{queen} + e_{woman} \approx e_{man}$) is true.

#### Reference:
*  Mikolov, Tomas, et al. "[Efficient Estimation of Word Representations in Vector Space](https://arxiv.org/abs/1301.3781)" Advances in neural information processing systems. 2013. 

## Spatial Data
### 1. Image Retrieval
 Use the trained ConvNet to perform image retrieval on the ood data. When using a certain image as query image, the remaining 4,999 images should serve as a retrieval date base. Perform image retrieval using neural codes from the same 3 layers which were also used in the paper by Babenko et al. Compare the results.

#### Reference:
* Artem Babenko, Anton Slesarev, Alexandr Chigorin, Victor Lempitsky, "Neural Codes for Image Retrieval"*, ECCV, 2014. https://arxiv.org/abs/1404.1777.

### 2.Triplet networks & one-shot learning
Train a Siamese network for one-shot learning task on the Omniglot dataset with triplet networks, and compare our model performance under different triplet selection method.

#### References:
* https://sorenbouma.github.io/blog/oneshot/ and https://github.com/sorenbouma/keras-oneshot/blob/master/SiameseNet.ipynb

## Sequential Data
### 1. Aspect-level Sentiment Classification
Build an attention-based aspect-level sentiment classification model with biLSTM. The model is trained bsaed on transferring learning such that first train your model on documnet-level examples. Then the learned weights will be used to initialize aspect-level model and fine tune it on aspect-level examples.


#### Reference:
* R. He, WS. Lee & D. Dahlmeier. Exploiting document knowledge for aspect-level sentiment classification. 2018. https://arxiv.org/abs/1806.04346.

### 2. Image Caption Generation
Construct a Long-Short-Term-Memory (LSTM) network which takes an image representation ob-tained from a convolutional neural network (ConvNet) as input, and produces a caption describing the image. 

#### Reference:
* Oriol Vinyals, Alexander Toshev, Samy Bengio, Dumitru Erhan,Show and Tell: ANeural Image Caption Generator, CVPR, 2015. https://arxiv.org/abs/1411.4555

## Generative models
### Anomaly Detection with VAEs
Use FashionMNIST to simulate the anomaly detection task. Omit one class from the training data, and consider the remaining 9 classes to be “normal”. The goal is then to identify the omitted class in the test data, by comparing the ELBO values obtained from a VAE trained on 9 classes.

#### Reference:
* Diederik P Kingma, Max Welling. Auto-Encoding Variational Bayes, 2013. https://arxiv.org/abs/1312.6114
