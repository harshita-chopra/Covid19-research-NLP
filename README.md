## Analysing the CORD-19 papers using NLP

Dataset Description
In response to the COVID-19 pandemic, the White House and a coalition of leading research groups have prepared the COVID-19 Open Research Dataset (CORD-19). CORD-19 is a resource of over 45,000 scholarly articles, including over 33,000 with full text, about COVID-19, SARS-CoV-2, and related coronaviruses. This freely available dataset is provided to the global research community to apply recent advances in natural language processing and other AI techniques to generate new insights in support of the ongoing fight against this infectious disease. There is a growing urgency for these approaches because of the rapid acceleration in new coronavirus literature, making it difficult for the medical research community to keep up.

The dataset is downloaded from https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge (Version 4, dated 20-03-2020)

My python program uses Natural Language Processing tools to clean the dataset and extract common phrases and word-cloud depicting the most talked about words. Another task of summarizing top 5 papers' body-text containing specific words according to the number of occurences is also done. The summarizer is created using word scoring by TF-IDF, a weight/statistical measure used to evaluate how important a word is to a document in a collection or corpus. The summary is made up of top 5 most weighted sentences. The related_papers function accepts a search word and displays the top summaries with paper IDs so as to access the entire paper if found useful.

The top papers regarding "Drug repurposing", "Chloroquine", "Atazanavir" and "Antiviral inhibitors" are extracted in this python notebook.
