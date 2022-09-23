Datasets and experimental results

Datasets from Previous Works (for generating synthetic sessions and training RQG models)

GCG dataset: contains painting passages from National Gallery Singapore (Proprietary)
RAB dataset: passages on Ranaissance paintings (https://www.britannica.com/list/25-famous-paintings-to-see-the-next-time-youre-in-florence)


Dataset     #Passages     #Sentences

GCG         21            3-10

RAB         25            7-15


Using these 46 passages, and our data augmentation technique, the number of utterance pairs for learning RQG = ~2.7K 


Performance of Answer Correctness Classifier (T5-large trained on SQuAD2.0) on manually-annotated (QA pairs from RoBERTa QA model on GCG/RAB)
![image](https://user-images.githubusercontent.com/58678112/191924482-b46489e9-790d-4c66-bcb3-f5a763381050.png)



Performance of TE approach (Convert QA to Declarative and do textual entailment with premise=answer containing statement)
![image](https://user-images.githubusercontent.com/58678112/191924407-95863781-b5e2-4891-9fdb-3b21e827aeb6.png)


User Evaluation

![image](https://user-images.githubusercontent.com/58678112/191927288-c3d32358-19cb-4c8b-b66b-75d155f702d1.png)




