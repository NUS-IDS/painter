Datasets and experimental results

Datasets from Previous Works (for generating synthetic sessions and training RQG models)

GCG dataset: contains painting passages from National Gallery Singapore (Proprietary)
RAB dataset: passages on Ranaissance paintings (https://www.britannica.com/list/25-famous-paintings-to-see-the-next-time-youre-in-florence)


Dataset     #Passages     #Sentences

GCG         21            3-10

RAB         25            7-15


Performance of Answer Correctness Classifier (T5-large trained on SQuAD2.0) on subset of manually-annotated (QA pairs)
![image](https://user-images.githubusercontent.com/58678112/191923862-45a9c61a-22b4-421e-857c-c19930b17e87.png)


Performance of TE approach (Convert QA to Declarative and do textual entailment with premise=answer containing statement)
![image](https://user-images.githubusercontent.com/58678112/191923961-11d448ac-023a-43d7-ba1b-29078ce74eb9.png)





