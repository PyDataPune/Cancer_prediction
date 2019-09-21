Problem Statement Classify the given genetic variations/mutations based on evidence from text-based Data.

Real-world objectives We have two data files: one conatins the information about the genetic mutations and the other contains the clinical data (text) that human experts/pathologists use to classify the genetic mutations. Both these data files are have a common column called ID

Download Data form here : - https://drive.google.com/open?id=1ZCewF6F3a21tK9yVjg2jnsdAbUwN3tl3

Data file's information:

training_variants (ID , Gene, Variations, Class) training_text (ID, Text) File descriptions training_variants - a comma separated file containing the description of the genetic mutations used for training. Fields are ID (the id of the row used to link the mutation to the clinical evidence), Gene (the gene where this genetic mutation is located), Variation (the aminoacid change for this mutations), Class (1-9 the class this genetic mutation has been classified on) training_text - a double pipe (||) delimited file that contains the clinical evidence (text) used to classify genetic mutations. Fields are ID (the id of the row used to link the clinical evidence to the genetic mutation), Text (the clinical evidence used to classify the genetic mutation)

Machine Learning Objective Objective:- Predict the probability of each data-point belonging to each of the nine classes.

Performance Metric - Multi class log-loss
