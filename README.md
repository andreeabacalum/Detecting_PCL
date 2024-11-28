# Detecting Patronising or Condescending Language in News Articles

## Table of Contents
- [Project Description](#project-description)
- [Data](#data)
- [Tech Stack](#tech-stack)
  
## Project Description

The aim of this project is to design a binary classification model to predict whether or not a text contains patronising and condescending language (PCL). PCL is defined as language which ”shows a superior attitude towards others or depicts them in a compassionate way” (Carla Perez-Almendros). As this kind of language is usually hard to detect, this is a challenging natural language processing task. Using the Don’t Patronise Me! dataset,
our goal is to develop and train a model which
outperforms in F1 score the performance of the
RoBERTa-base baseline model of task 4, from the
SemEval 2022 competition.

## Data 

The model is trained on the dontpatronizeme
pcl.tsv dataset. This dataset is comprised of
10,469 paragraphs, which were selected from various news articles about potentially vulnerable social groups, which include the disabled, homeless,
hopeless, immigrant, in need, migrant, poor families, refugee, vulnerable and women communities.
All the paragraphs have been annotated with labels
which depict the level of PCL they contain: from
0 (not containing PCL at all) to 4 (the paragraph is
very patronising and condescending towards vulnerable communities). Each paragraph has been
annotated by 2 annotators with either 0 (No PCL),
1 (borderline PCL) and 2 (contains PCL), and their
results have been summer up into a label for each
paragraph. For our task, we consider paragraphs
with label in {0,1} as not PCL, and paragraphs
with label in {2,3,4} as PCL.


## Tech Stack

The entire project was built using Python
