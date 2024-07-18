# image-to-json

# Finetuning PaliGemma for image to JSON use cases

In this repo, I've finetuned Google's PaliGemma, an open vision-language model, on a custom dataset where the goal for the model is to turn a receipt image into a JSON containing all fields.

<img src="https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/blog/paligemma/paligemma_arch.png"
alt="drawing" width="600"/>

- Used huggingface datasets for loading the dataset and Pytorch lightning for training the model

- In order to train the model in a parameter-efficient way, leveraged the huggingface PEFT library (Parameter-Efficient Fine-tuning) along with Accelerate and Bitsandbytes

- Also used Weights and Biases for logging (seeing our loss going down during training)
