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
# Milestone 1
- Readline; reads one line and identifies spaces in the line
- Trigram; splits line 3 characters at a time and records the data
# Milestone 2
- Similarity; counts the number of similarities between trigrams
  -references the cosine similarity class
  - uses the reference to show similarity as either a 1 or 0 indicating if it is a match
- Frequency; records trigrams that occur more than once and totals them
- (Possible)Compare; Compares test file trigram frequency and training data profile similarities
### Main Formats
#Milestone 1
-Main() to test frequency of trigrams
  -Takes data from Frequency function (trigram totals, similarities)
  -Prints number of times that trigrams occur in the file
#Milestone 2
-Main() to test which filename of the training data input has the most similarities
  - Will take lines read and trigram frequency data
  - Will compare input file names and output which profile has the most similarities
## Files Needed
- Cosine Similarity cpp file; used to reference in Milestone 2
## Libraries Needed
-vector
-string
-"CosineSimilarity"
## Compile
- main.cpp
-"CosineSimilarity.cpp"
