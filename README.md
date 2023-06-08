# Readme
This is a machine annotator for Japanese free text incident reports of medication errors. This pipeline has been tested to be stable and works best on Google Colab. The machine annotator utilizes CUDA, so please set the Runtime type to 'GPU'.

### SETUP:
(1) Please mount the shared files (including "wiki-ja.model", "config.json", "model_entity_220309.bin", and "model_3_220310_2.bin") accordingly into "TOKENIZER_MODEL", "BERT_CONIFG_FILE", "BERT_PRETRAINED_MODEL", "MODEL_SAVE_PATH".

(2) Next please set up input/output file paths:
  - "in_dir": the input file path, it should be a xlsx file with two columns: "id" and "report", saved in the "freetext" sheet. 
  - "out_dir": the output file path, it will generate the entity-level predicted output from the trained machine-annotator.

### RUN:
Please run the code chunk by chunk and you will find the entity-level annotation in "out_dir".

For any inquiries, please email to Dr Zoie SY Wong (zoiesywong@gmail.com)
