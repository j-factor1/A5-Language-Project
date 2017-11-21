#Design Document for Language Detection
##Jackson Factor
##jackson_factor@my.uri.edu

##Problems to Solve
## Milestone 1
-Using cosine similarity to identify matches in Language
-Recognizing frequencies using trigrams
-Creating a one line command argument to read the line and identify spaces
-Recording instances of different trigrams and letters frequencies
## Milestone 2
-Writing program to take two or more command lines
-Recognizing frequency of trigrams in training data, n-1
-Compute trigram frequency for test file
-Determine which training files profile is most similar and output the file's name
##Classes Needed
- A Cosine Similarity Class
  -Recognizes similarity instead of distance in equation
  -Ranges from 0 to 1 showing either a match or nothing
  -Larger cosine similarities show better matches
##Other Functions
