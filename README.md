# Notebook Descriptions

This repository contains Jupyter notebooks used in the dissertation **Analysis of the impact of Quantization on Pre-Trained Transformer Models**.

The notebooks can be grouped as follows:

## Pretrained Model Details

The notebook **Pre_trained_model_details** downloads and prints the details of the pre-trained models used in this dissertation.

## Inference on original models

These notebooks implement inference on the original version of the models, which are later quantized as part of this study. This is to allow comparison with quantized versions of those models.

- **Llama-2-7b-chat-hf_inference**
- **Llama-2-7b-hf_inference**
- **Mistral-7B-Instruct_inference**
- **Falcon-7b-instruct_inference**

## Quantization of pre-trained models

This set of notebooks quantizes a model and then runs inference on the quantized model. It also uploads the model to the Hugging Face Hub.

- **Quantize_falcon_7b_instruct_NF4**
- **Quantize_Llama_2_7b_chat_hf_AWQ**
- **Quantize_Llama_2_7b_chat_hf_NF4**
- **Quantize_Llama_2_7b_chat_HF_AutoGPTQ**
- **Quantize_Mistral_7B_Instruct_NF4**

## Model Evaluation

These two notebooks evaluate the models. Both the original models and the quantized models are evaluated in their respective notebooks using the benchmarks MMLU, HellaSwag, BoolQ, and BBH.

- **Evaluation_of_original_models**
- **Quantized_Model_Evaluation**

## Original Vs Quantized

These notebooks run inference on the original models and quantized versions of those models in the same notebook to allow for a direct comparison.

- **Original_vs_quantized_Llama_2_7b_chat_hf**
- **Original_vs_quantized_Llama_2_70b_chat_hf**

## Fine-tuning

The notebook **Fine_tune_llama2_hf_NF4_with_QLORA** demonstrates how to fine-tune models using quantization and the PEFT technique QLORA.
