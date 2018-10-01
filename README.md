# Search-Engine-Evaluation
Project done for the Data Mining Technologies. The main topics covered in this project are Search-Engine Evaluation and Near-Duplicates-Detection.

You may check out the report.pdf part in which I have described the different results obtained from the evaluation.

## Part 1
In this part of the homework, you have to assess the quality of three different Search-Engines using only the ground-truth and their query-results.

## Part 1.1
Using the data available in dataset/part_1_1/, assess the quality of the three Search-Engines using the following evaluation metrics: P@k, R-Precision, MRR (Mean Reciprocal Rank) and nDCG.

## Part 1.2
The “NoobDataScience” company needs to select the best Search-Engine module, among three modules, for its latest successful app: “TetraSocialApp”. Data from these three Search-Engine modules are located here: dataset/part_1_2/ .
For assessing the quality of the Search-Engine modules in a correct way, you have to consider that the app provides in output only four results for each search query. Moreover, these four results are displayed in random positions on the smartphone screen.
Which is the best Search-Engine module for the app?

# Part 2
In this part of the homework, you have to deal with three data mining problems: Near-Duplicate-Detection, Set-Size-Estimation and Unions-Size-Estimation problem.
 
You have to find, in an approximated way, all near-duplicate documents inside the lyrics dataset
Each html represent the lyrics of a song, that is contained only in the html body.
For this part of the homework, you must consider two documents as near-duplicates if, and only if, the jaccard between their associated sets of shingles is ≥0.85.

### Details on Shingling
For each document, the set of shingles must be a set of natural numbers.
Before shingling a document, it is required to remove punctuations and convert all words in lower-case. The length of each shingle must be 3.
You have to shingle only the lyric of the song.
### Details on Sketching
Constraint 1: Each set of shingles, that represents an original document, must be sketched in a Min-Hashing sketch of length 300.
### Details on LSH
Constraint 2: It is acceptable to have as a near-duplicates candidate a pair of documents with Jaccard=0.85, with probability ≥ 0.97.
Constraint 3: Of course, you have to reduce as much as possible the number of candidate pairs to be near-duplicates, by keeping constraint 1 and 2 satisfied.

## Goals
It is requested to achieve the following three goals by satisfying the constraints presented in the previous paragraphs:
1. Report the near-duplicates you found.
2. Report the set of near-duplicate candidates you found.
3. Report the False-Positive that have been filtered out.




