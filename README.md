# PytArt
Engineered Art in Python

PytArt is a personal project to practice my Python skills on creative art projects. The first (and for now the only) .py script converts a poem into colorful blocks, where the colors are based on the rhymes between the words. 

The poems already have certain visual structures, such as stanzas, number of words in a line, and number of letters in a word. These visual cues give the reader an initial perception on the poem.

This script takes a string (e.g. a poem) and evaluates a unique code for each word based on the number of each letter in the alphabet. This yields a dataset with 26 features (number of letters in the English Alphabet). The dataset is reduced down to 3 features by principal component analysis. Here, the first three principal components with the most variance will capture the similarities (mostly phonetic, but not always. Works better in my native language, Turkish.) between the words. Hence, the projection of the words on these principal components are accepted as the RGB code to represent the words in colors. 

The resulting abstract figure shows the similarities between the words, ergo the structure of the poem that a naked eye may not capture at a first glance.

The posted script visualizes The Raven by Edgar Allan Poe, one of my favorites in American literature.
