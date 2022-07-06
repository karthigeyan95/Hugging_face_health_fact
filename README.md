# Hugging_face_health_fact
Built a text classification model to verify the varacity of the medical claims using pretrained transformer models. Used Huggingface framework to fine tune the BERT transfer learning model.

About the Data

PUBHEALTH is a comprehensive dataset for explainable automated fact-checking of public health claims. Each instance in the PUBHEALTH dataset has an associated veracity label (true, false, unproven, mixture).

training data class distribution
Unproven - 5078
true - 3001
false - 1434
mixture - 291

1. Setup (Used Colab GPU for Training)

I was not able to use my system's resources to train the model so used Google Colab offers free GPUs. Since we’ll be training a large neural network it’s best to take advantage of this (in this case we’ll attach a GPU), otherwise training will take a very long time.

2. Installing the Hugging Face Library and other necessary libraries.

3. Loading health fact Dataset from the list of 935 datasets available in huggingface.

4. Tokenization of the input (To feed our text to BERT, it must first be divided into tokens, which must then be mapped to their index in the tokenizer vocabulary. The tokenizer included with BERT must perform the tokenization.)

5. Splitting the data into Training & Validation Split

6. Optimizer & Learning Rate Scheduler (After loading the model we have to set the training hyperparameters needed for the model to train.

7. Train the model and validate its loss on both training and validation sets

8. Test the performance of the model on the test set
