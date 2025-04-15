## **Notes**
### **Week 1***
Goal 
1) from RNA sequencing, produce a model that tells me if there is TP53 mutation or not.
2) specify which type of mutation

We need to have mutation data, sequencing data and type of mutation.

Question 1: is TP53 mutation affecting the RNA at all? 

Question 2: is the type of mutation in TP53 affecting the RNA sequencing or not?

### **Week 2**
We have RNA and DNA sequences. The cell has the nucleus and DNA from nucleus is transcribed into RNA, which procesess into proteins (not all RNA become proteins but we don't care). 

Transcription Factors are proteins that work inside the nucleus. They bind to the DNA and start transcription. 

Our task is to understand how the annotation in one of these proteins affects the RNA. In particular, our protein is TP53 (the guardian of the Human Genome), which stops the cell when there is a damage. Obviously in cancer it is very mutated -> we have a lot of public data. 

TP53 can be white type or muted. Since it triggers the transcription of many RNAs, we expect that from the RNA signal we should be able to detect whether there is a mutation of TP53. 

We should use the databases where we have the DNA / RNA sequences already processed (not raw data) where we have whether the gene is mutated or not. 

First task is binary classification (whether the gene is mutated or not). After this, we need to predict also the type of mutation. When we get to this second task we can look online and we will see that there are databases for different types of mutations.
