# GAN-BERT (PyTorch)

## Background
Quality labelled datasets are hard to come by, and this makes deep learning difficult as many techniques require at least thousands of records for a model to train and perform well. As such, few-shot classifiers can be considered, and one of these is the GAN-BERT.

GAN-BERT is an extension of the original BERT model supported by a Generative Adversarial Network (GAN). It is fine-tuned with both real data and fake data, the latter of which is created by the Generator. The model then uses the Discriminator to classify the data into its classes and if the data is real. Overall, the researchers behind GAN-BERT suggest that it requires substantially lesser labelled data than its original counterpart, and this helps to alleviate the issue of a lack of quality data.

## Code

This GAN-BERT model was fine-tuned on the **ISEAR dataset** (7,500 records) across the **emotions/classes of 'unk', 'anger', 'disgust', 'fear', 'guilt', 'joy', 'sadness', 'shame'**, and its code was adapted from that in its original repository, which also contains a more detailed explanation of its theoretical underpinnings.

https://github.com/crux82/ganbert-pytorch

## Results

The results were only comparable (in terms of **Recall**) to those achieved by BERT. For more details on the results of the latter, refer to this repo:

https://github.com/tobys-playground/fine-grained-sentiment-analysis
