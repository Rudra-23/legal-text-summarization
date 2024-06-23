<h2> The Future of Legal Reviews: Fine-tuning LLMs for Efficient Legal Text Summarization </h2>

Legal documents are characterized by their verbose and complex nature, often containing technical language that poses a barrier to comprehension for the layperson. To address this challenge, we propose a novel approach leveraging custom-trained Large Language Models (LLMs) for summarizing legal documents.

Model: https://huggingface.co/Rud/LED_multi_lexsum_peft

Dataset: https://huggingface.co/datasets/allenai/multi_lexsum

<h4> Results </h4>

T5: fine-tuned on text of length 512 tokens.
BART: fine-tuned on text of length 1024 tokens.
LED: fine-tuned on text of length 4096 tokens.

| Model            | Stage       | Rouge-1 | Rouge-2 | Rouge-L |
|------------------|-------------|---------|---------|---------|
| T5 Model         | Pre-trained | 0.0179  | 0.0064  | 0.0166  |
| T5 Model         | Fine-tuned  | 0.1970  | 0.1064  | 0.1667  |
| Distil-BART Model| Pre-trained | 0.3027  | 0.1104  | 0.1740  |
| Distil-BART Model| Fine-tuned  | 0.4405  | 0.2521  | 0.3143  |
| LED Large Model  | Pre-trained | 0.3104  | 0.0766  | 0.1400  |
| LED Large Model  | Fine-tuned  | 0.3657  | 0.1149  | 0.1682  |

<h4>Conclusion</h4>

Our project has effectively utilized advanced
encoder-decoder models such as T5-Small, DistilBart, and the LED-Large Model, all trained on
the specialized Multi Lexsum dataset to enhance
legal document summarization. This multifaceted
approach has led to notable improvements in the
quality of summaries across all models.

Finally, on our latest model, we achieved a bert-score F1 of 0.83 on test dataset. 
