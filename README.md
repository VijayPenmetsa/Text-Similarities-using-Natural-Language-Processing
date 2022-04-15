# Text Similarities using Natural Language Processing

## Introduction

In this project we explore various Natural Language Processing technologies, to accurately compare and find out **similarities between different textual data**. These techniques can be used to easily search for similar words in a given text. 
After finding the **similar words**, we **visualize** the results based on their similarity index using **Radar Charts.**

The libraries used in this project:
- **_Sentence Transformers_** _(based on pytorch and transformers)_
- **_Textacy_** (built on high-performance spaCy library)
- **_Numpy_**
- **_Pandas_**
- **_Plotly_**


## Files

**text_similarities.ipynb** 
This notebook contains the necessary code for finding similarities between text, and visualizing them.


## Data 

For this we have used 2 different paragraphs from **Wikipedia.**

The 2 paragraphs are:
1. **Description of Audi.**
2. **Description of BMW.**


## Extracting top 5 keywords from each description using spaCy.

<img width="1052" alt="Screen Shot 2022-04-14 at 9 45 40 PM" src="https://user-images.githubusercontent.com/50517893/163504932-2f81b2a0-9a7f-43d5-a849-40bd141221e8.png">

Here, using textacy we extracted the top keywords from each of the descriptions.

## Calculation and Visualization of similarities

**Calculation:**
- Now that we have the keywords, we need to calculate their cosine similarities and compare them against each other.
- Next we get the text embeddings using the model **_SentenceTransformer('stsb-roberta-large')_**.
- We then use these text embeddings to calculate the cosine scores using the function **_pytorch_cos_sim()_** 

### The following is a visualization of most similar words from both of the top 5 keyword lists.

<img width="1103" alt="Screen Shot 2022-04-14 at 10 05 57 PM" src="https://user-images.githubusercontent.com/50517893/163506418-f7370f93-b114-4e87-b66d-57dbbd295e4b.png">
 
 
### Next visualization is about the the similarities of all the top keywords in both the paragraphs (Audi and BMW).


<img width="1458" alt="Screen Shot 2022-04-14 at 10 06 27 PM" src="https://user-images.githubusercontent.com/50517893/163506590-10fb9548-8351-4ff9-a1dc-da3dbacf3379.png">










