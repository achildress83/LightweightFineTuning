# Applying LoRA to distilbert
This project demonstrates applying a parameter efficient fine-tuning technique to a foundation model to adapt the pre-trained model to the downstream classification task of phishing detection. In this case, I'm using Low-Rank Adaptation (LoRA) to fine-tuning [distilbert](https://huggingface.co/docs/transformers/en/model_doc/distilbert) (a small version of BERT) to classify text as phishing or benign.

I first evaluate the base distilbert model (without finetuning) to assess its performance - performance is about what you'd expect from a random guess.

I then train adapter weights using LoRA, with achieves over 90% accuracy after only two epochs.

Dataset: [phishing dataset](https://huggingface.co/datasets/ealvaradob/phishing-dataset)
