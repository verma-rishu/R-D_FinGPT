# Reseach and Development on FinGPT

**What is FinGPT?**

**FinGPT** [[1]](https://arxiv.org/abs/2306.06031) is an **open-source** large language models (LLMs) focused on finance. This open-source LLM is developed using a data-driven approach and by using various open-source LLMs as the base model, which are further finetuned on any specific financial dataset. The performance of the fine-tuned model can be further enhances with techniques like LoRA, instruction-tuning, RAG, etc. which not only show improved performance in terms of accuracy but also significantly reduce the cost of training and inference.

Summary of the results from the notebooks in this repo:

<table width="100%">
  <tr>
    <td>Notebook</td>
    <td>Base Model</td>
    <td>Epochs</td>
    <td>GPU</td>
    <td colspan="2">Results_TFNS</td>
     <td colspan="2">Results_FPB</td>
     <td colspan="2">Results_FiQA</td>
     <td colspan="2">Results_NWGI</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td>Accuracy</td>
    <td>F1 (weighted)</td>
    <td>Accuracy</td>
    <td>F1 (weighted)</td>
    <td>Accuracy</td>
    <td>F1 (weighted)</td>
    <td>Accuracy</td>
    <td>F1 (weighted)</td>
  </tr>
  <tr>
    <td><a href="https://github.com/verma-rishu/R-D_FinGPT/blob/main/FinGPT_ChatGLM2_6B.ipynb">FinGPT_ChatGLM2_6B</a></td>
    <td><a href="https://huggingface.co/THUDM/chatglm2-6b">chatglm2-6b</td>
    <td>3</td>
    <td>Google Collab A100 GPU <small>(approx: 30-35 compute units for training ~ 5-7 for inference)</small> </td>
    <td>0.889</td>
    <td>0.889</td>
    <td>0.789</td>
    <td>0.774</td>
    <td>0.621</td>
    <td>0.774</td>
    <td>0.621</td>
    <td>0.688</td>
  </tr>
  <tr>
    <td><a href="https://github.com/verma-rishu/R-D_FinGPT/blob/main/FinGPT_Llama2_7B.ipynb">FinGPT_Llama2_7B</a></td>
    <td><a href="https://huggingface.co/meta-llama/Llama-2-7b-chat-hf">llama2-7b</td>
    <td>2</td>
    <td>Google Collab A100 GPU <small>(approx: 45-50 compute units for training ~ 10-11 for inference)</small> </td>
    <td>0.684</td>
    <td>0.593</td>
    <td>0.643</td>
    <td>0.545</td>
    <td>0.174</td>
    <td>0.193</td>
    <td>0.441</td>
    <td>0.335</td>
  </tr>
      <tr>
    <td><a href="https://github.com/verma-rishu/R-D_FinGPT/blob/main/FinGPT_Llama2_13B.ipynb">FinGPT_Llama2_7B</a></td>
    <td><a href="https://huggingface.co/NousResearch/Llama-2-13b-hf">llama2-13b</td>
    <td>2</td>
    <td>Google Collab A100 GPU <small>(approx: 85-90 compute units for training ~ 10-11 for inference)</small> </td>
    <td>-</td>
    <td>-</td>
    <td>0.873</td>
    <td>0.873</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
    <td>-</td>
  </tr>
</table>

Datasets (for inference) [[3]](https://arxiv.org/abs/2307.10485):
- TFNS - Twitter Financial News Sentiment Validation (Twitter Val)
- FPB - Financial PhraseBank
- FiQA - Financial Question Answering
- NGWI - News with GPT instructions
  
Papers referred:
1. [FinGPT: Open-Source Financial Large Language Models](https://arxiv.org/abs/2306.06031)
2. [Instruct-FinGPT: Financial Sentiment Analysis by Instruction Tuning of General-Purpose Large Language Models](https://arxiv.org/abs/2306.12659)
3. [FinGPT: Democratizing Internet-scale Data for Financial Large Language Models](https://arxiv.org/abs/2307.10485)

Github references:
-  [AI4Finance-Foundation/FinGPT](https://github.com/AI4Finance-Foundation/FinGPT)
-  [AI4Finance-Foundation/FinNLP](https://github.com/AI4Finance-Foundation/FinNLP)

