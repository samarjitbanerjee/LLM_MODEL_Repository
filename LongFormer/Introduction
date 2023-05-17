LONGFORMER-BASE-4096 fine-tuned on SQuAD v1
This is longformer-base-4096 model fine-tuned on SQuAD v1 dataset for question answering task.

Longformer model created by Iz Beltagy, Matthew E. Peters, Arman Coha from AllenAI. As the paper explains it

Longformer is a BERT-like model for long documents. 

The pre-trained model can handle sequences with upto 4096 tokens.

Few things to keep in mind while training longformer for QA task, by default longformer uses sliding-window local attention on all tokens. But For QA, all question tokens should have global attention. For more details on this please refer the paper. The LongformerForQuestionAnswering model automatically does that for you. To allow it to do that

The input sequence must have three sep tokens, i.e the sequence should be encoded like this <s> question</s></s> context</s>. If you encode the question and answer as a input pair, then the tokenizer already takes care of that, you shouldn't worry about it.
input_ids should always be a batch of examples.
Results
Metric	# Value
Exact Match	85.1466
F1	91.5415
