# Statistical-Machine-Learning---Computer-Vision

In the Deep Learning community, we may have some pointers for coming up with useful architectures of deep neural networks but there still is no consensus that details reasons about architectural choice [1,2,3,4,5]. In this project, we want to focus on the advantages and disadvantages of network design choices. Since deep learning spans a plethora of research directions, we would like to focus on the architectures and application areas that brought it a significant amount of attention in recent years. Specifically, we want to pick one of the datasets like Imagenet[3], or CIFAR10 / CIFAR100 (image-based datasets) and compare the architectures via metrics like Accuracy, Precision, Recall, F-1, ROC, AUC and robustness measures (like by adding noisy training data). We implement EfficienctNetV2 which is a new family of CNNs that have faster training speed, better accuracy and smaller models. We also explore transformer architecture which is extremely popular with NLP tasks, but there are only limited applications in the field of Computer Vision. So we implement techniques like attention in conjunction with CNN's and even replace components of the CNN network with attention layers. We also show that this reliance on CNN is not essential, and a pure transformer network (ViT, Vision Transformer) can be used to achieve SOTA accuracy. While ViT has great accuracies, they are computationally expensive and compromise on the integrity of 2-D data (images) by flattening them, so we explore Signal Processing techniques through WaveMix (Multi-resolution Token mixing for images) which addresses these issues while achieving similar results in a much more compute-efficient way even when compared to CNNs. Finally, we also go through the dropout approximation model averaging approach in which we create a simple new model called maxout that is meant to help dropout optimize and increase the accuracy of the rapid approximation model averaging approach used by dropout.
Of course, this project touches on many aspects of why a certain architecture should be better suited for the task, and we would want to test and justify the existing hypothesis about architecture preferences empirically.

Comparison Models:
LeNet, DenseNet, AlexNet, ResNet, VGG, Attention CNN, EfficienctNetV2, WaveMix and Vision Transformers, Maxout Networks.
