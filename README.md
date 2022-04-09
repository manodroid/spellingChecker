# spellingChecker
A simple spell checker using Norvigs algorithm for generating mutations and using the JaccardIndex Coefficient

This was a small school project about String manipulation and File managment. The idea is simple we create a dictionary by reading a file 
of the most common english words into a HashSet. I choosed this collection because it has O(1) for both insetion and lookup.
The program waits for input from the user and searches that input in the set, if the input ins't found we call the norvig function.
What this function does is that it generates other words from the input by deleting, inseting, or reversing the characters in the string, 
after we generate all the mutations of the word we keep only those that are in the dictonary.

Then we calculate the similarity of each suggestion with the word by using the Jaccard Index wich compares the set of characters of the 
input and each suggestion. This way we only use the words with the biggest similarity.

TO-DO:
  Improving the search time using a Bloom Filter.
  Improving the space complecity by generating fewers words.
 
