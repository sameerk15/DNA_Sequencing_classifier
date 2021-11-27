
# DNA_Sequence_Classifier

DNA or Deoxyribonucleic acid is a hereditary material in human beings and in every other living organism. The information in DNA is stored in the form of code made of four chemical bases i.e. Adenine(A), Guanine(G), Cytosine(C), Thymine(T). 

The long DNA sequences are made of a combination of these 4 bases and each sequnce belongs to a particular class (0-6) and each class has different gene functionalities. eg.) AGTCGCATCGCTA, TCCGAATGCCGT etc.

The main objective of this project is to identify the class which those long sequences belongs to.
 
Our independent variable(X) is sequence and dependent variable(y) is the class label(0-6) i.e. Multi class classification. 


## Roadmap

Let us understand the basic approach of this project :

1) Importing dataset and libraries.
2) Apply k-mers counting on the sequences 
3) Apply Bag of words on result after applying k-mers to convert into vectors.
4) Build Multi Naive Bayes model.

Let us understand k-mers technique in detail.

Our task is to convert those sequences into some sort of vectors so that our model understands it.

The first thing that comes to mind is applying some Bag of words, TF-IDF or embeddings but all the sequnces are not of the same length. 

So, therefore we use a different technique called as K-mers technique.

Now what is k-mer technique?

In k-mers technique, we convert each DNA sequence into fixed size subsets(k-mers) of a fixed length(eg.6) and then apply Bag of words all those subsets.

For example, we have a dna sequence AGTCTGCAGCAT and we want to apply k-mer technique on this.

We decide that the fixed length will be 6(hexmers) so we first take the first 6 bases of original base and then we take the next 6 bases(overlapping allowed) excluding the first base and this process continues till we reach the end of sequence.

We apply this k-mers function to all the sequences.

We now have the fixed vector size for each sequence and we can apply Bag of words .


## Tech Stack

**Programming Language:** Python 3

**Libraries:** Pandas, Numpy, Seaborn, Matplotlib, CountVectorizer, Scikit-learn.

**Model:** Multinomial Naive Bayes


## Lessons Learned

One of the most important takeaway from the project is how AI is applied in Genomics and in the study of Genes and heriditary since this project is focused on Genomics. 

K-mers counting technique was a new approach that I learn to solve problems which have these kind of long sequences.
## Applications

This project has its application in:

- This is beneficial for Geneticists who study genes and hereditary.

- Used for medical purposes.


## Acknowledgements

 - [Genomics](https://www.nature.com/subjects/genomics)
 - [k-mers counting](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-12-333)
 - [Bag of words](https://machinelearningmastery.com/gentle-introduction-bag-words-model/)


## Authors

- [Sameer Kumar](https://github.com/sameerk15)

