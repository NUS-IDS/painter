# Asking Reflective Questions in ArtMuse


This repository is for hosting the resources and code designed for asking reflective questions in ArtMuse.

(AAAI demo track)


A demo version is available at https://nlp-platform.online/artmuse

QANLI dataset is described in https://arxiv.org/abs/1809.02922. This dataset
was used to learn to convert (QA) pairs to declarative sentences, that are used for textual entailment check/answer correctness.

Most of our models are based on the Text-To-Text Transfer Transformer or T5 (https://huggingface.co/t5-large)
described in this paper: https://jmlr.org/papers/volume21/20-074/20-074.pdf


Guides based on which the generic cues and question templates were designed:
https://www.terraamericanart.org/wp-content/uploads/2015/08/Terra-Discussing-Art-and-Anchor-Standards.pdf

https://www.nemanet.org/files/4813/8552/9230/Neurodiversity_1.pdf

# Machine and Model configuration details 
We performed all experiments on
a single GPU of an Nvidia Tesla cluster machine. 

Source/target lengths for RQG model = 64/24

PersonaChat dialog model = 512/32

Converting QA pair to Declarative Sentence (QANLI dataset) = 128/64

We fine-tune 
the T5-large model from HuggingFace (https://huggingface.co/t5-large) for
3-5 epochs. On the larger dataset (PersonaChat and QANLI), the training
time is around ten hours and for our smaller RQG dataset, the training time is about 30 minutes.

The batch size is set to 4, learning rate and eps parameters for the Adam optimizer are 1e-4 and 1e-8, respectively




Datasets for RQG obtained from previous work: https://ojs.aaai.org/index.php/AAAI/article/view/21519

The GCG collection is proprietary but the passages in the RAB collection are 
available at https://www.britannica.com/list/25-famous-paintings-to-see-the-next-time-youre-in-florence

#Overall Pipeline

![image](https://user-images.githubusercontent.com/58678112/191934223-bf4ea9af-70fd-4bce-aac8-dcdd9c7fe5b6.png)



